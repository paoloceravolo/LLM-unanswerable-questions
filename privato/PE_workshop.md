# Workshop: Comprendere i Limiti degli LLM per Utilizzarli Meglio

## 1. Introduzione

### Cosa sono gli LLM e come funzionano

I Large Language Models (LLM) sono modelli di intelligenza artificiale addestrati su enormi quantità di testo che possono generare linguaggio naturale in coerenza con alcune istruzioni. Il meccanismo fondamentale con cui apprendono si basa sul **masking**: durante l'addestramento, alcune parole vengono nascoste e il modello deve imparare a prevederle dal contesto.

**Semplice esempio di masking:**

Frase originale: "Il gatto dorme sul divano"

Durante l'addestramento:
- "Il gatto _____ sul divano" → il modello impara a prevedere "dorme"
- "Il _____ dorme sul divano" → il modello impara a prevedere "gatto"
- "Il gatto dorme _____ divano" → il modello impara a prevedere "sul"

Ripetendo questo processo miliardi di volte su quantità enormi di testo, il modello sviluppa una comprensione statistica del linguaggio: quali parole tendono a comparire insieme, quali strutture grammaticali sono comuni, quali concetti sono correlati. Quando riceve una richiesta, il modello utilizza questa conoscenza per generare una risposta che segue la sequenza di parole più probabile.

**Il loro compito di base è quindi legato al completamento di testi.** I primi modelli, limitandosi solo a questa capacità senza utilizzare altri strumenti, incontravano una serie di difficoltà significative:

- **Calcoli matematici**: non potendo usare una calcolatrice, dovevano "indovinare" il risultato basandosi su pattern visti durante l'addestramento.
- **Informazioni aggiornate**: senza accesso a internet, la loro conoscenza rimaneva congelata alla data di addestramento.
- **Verifiche fattuali**: senza possibilità di controllare fonti esterne, potevano generare informazioni plausibili ma inventate.

I modelli moderni hanno superato molte di queste limitazioni integrando strumenti esterni (calcolatrici, motori di ricerca, accesso ai database), ma comprendere la loro natura di "*completatori di testo*" ci aiuta a capire dove possono ancora incontrare difficoltà e perché determinate tipologie di domande rimangono problematiche.

### Le domande difficili per gli LLM

Non tutte le domande sono uguali per un LLM. Alcune tipologie di quesiti risultano particolarmente sfidanti e possono portare a risposte errate o imprecise. Identificare queste difficoltà è fondamentale per diversi motivi:

- **Comprendere il "ragionamento"**: capire dove gli LLM falliscono ci aiuta a capire come elaborano le informazioni.
- **Utilizzo più efficace**: conoscendo i limiti possiamo formulare richieste più appropriate.
- **Valutazione critica**: possiamo riconoscere quando una risposta potrebbe essere inaffidabile.

## 2. Obiettivi del workshop

Fornire ai partecipanti una comprensione pratica e operativa delle limitazioni intrinseche dei Large Language Models (LLM) nello specifico contesto della formulazione delle domande, e dotarli degli strumenti metodologici per progettare prompt robusti, efficaci e resilienti.

### Obiettivi di apprendimento specifici

#### 1. Tassonomia delle domandepProblematiche
*   **Identificare** e **classificare** le principali categorie di input che inducono in errore gli LLM (es. domande ambigue, contraddittorie, con presupposti falsi, fuori contesto temporale/spaziale).
*   **Comprendere** le ragioni tecniche e cognitive (bias nei dati di training, architettura del modello) alla base di queste vulnerabilità.

#### 2.  Valutazione empirica
*   **Sperimentare attivamente** con diversi modelli di LLM (es. GPT-5, Claude, Gemini, modelli open-source) utilizzando un set condiviso di domande critiche.
*   **Valutare** e **confrontare** le performance, i punti di forza e le debolezze specifiche di ciascun modello in scenari problematici.
*   **Documentare** le risposte in modo sistematico per identificare pattern di errore e resilienza.

### 3. Sviluppo di competenze pratiche nel prompt engineering
* **Capire e sperimentare** come scrivere richieste efficaci per un’IA:
  * **Spezzare un problema** in più domande semplici.
  * **Dare un ruolo all’IA** (es. “comportati come un tutor”, “come un giornalista”).
  * **Usare esempi** per far capire meglio cosa si vuole ottenere.
  * **Chiedere risposte ragionate**, passo dopo passo, quando serve.
  * **Tenere conto della conversazione**, ricordando cosa è già stato detto.
* **Provare a migliorare un prompt** facendo piccoli cambiamenti e osservando cosa cambia nella risposta.
* **Costruire prompt riutilizzabili**, come modelli di partenza da adattare a situazioni diverse.

---

## 3. Principi generali per scrivere un buon prompt

Prima di esplorare le categorie problematiche, ecco alcune linee guida fondamentali:

1. **Essere specifici e chiari**: evitare ambiguità nella formulazione.
2. **Fornire contesto**: includere informazioni rilevanti per la risposta.
   - Se invece non conosciamo un contesto adeguatamente è meglio restare generici per evitare di indirizzare l'LLM in una direzione sbagliata.
3. **Strutturare le richieste complesse**: suddividere domande articolate in passaggi.
4. **Specificare il formato desiderato**: indicare come si vuole ricevere la risposta.
5. **Utilizzare esempi (ma con cautela)**: gli esempi possono essere molto utili per chiarire cosa si vuole, ma attenzione:
   - L'LLM potrebbe replicare troppo letteralmente lo stile o formato dell'esempio.
   - Esempi limitati possono restringere artificialmente lo spazio delle risposte possibili.
   - Il modello potrebbe cogliere pattern non intenzionali dagli esempi forniti.
   - **Quando usarli**: per compiti creativi o quando il formato è fondamentale.
   - **Quando evitarli**: quando si vuole esplorare soluzioni diverse o si cerca completezza.

## 4. Tassonomia delle domande difficilie per gli LLM 

[Tassonomia delle domande difficili ](./tassonomia_domande.md)

---

## 5. Gestione della attività

### Fase 1: Esplorare i limiti degli LLM open-source

**Obiettivo**: Testare modelli open-source meno avanzati per identificare punti deboli evidenti.

**Istruzioni:**
1. Formare gruppi di 3-4 persone
2. Ogni gruppo riceve una categoria specifica di domande difficili
3. Il compito è creare una domanda che:
   - Appartenga alla categoria assegnata.
   - Porti l'LLM a rispondere in modo scorretto.
   - Oppure porti l'LLM a non riconoscere di non saper rispondere.
4. Testare la domanda su un modello open-source fornito.
5. Documentare la domanda e la risposta ottenuta.

**Tempo**: 15-20 minuti

**Modelli suggeriti**: GPT-OSS 2, DeepSeek-r1, o modelli simili disponibili localmente

### Fase 2: Sfidare gli LLM avanzati in cloud

**Obiettivo**: Verificare se modelli più sofisticati superano le stesse sfide o presentano limiti diversi.

**Istruzioni:**
1. I gruppi ricevono una nuova categoria (diversa dalla prima)
2. Ripetere l'esercizio, ma questa volta utilizzando LLM avanzati in cloud
3. L'obiettivo è creare domande che mettano in difficoltà anche questi modelli
4. Confrontare i risultati con quelli della Fase 1

**Tempo**: 15-20 minuti

**Modelli suggeriti**: ChatGPT-5, Claude-3, Gemini-3, o equivalenti

### Fase 3: Condivisione e discussione

**Domande guida per la discussione plenaria:**

1. **Quante domande "problematiche" è riuscito a creare ogni gruppo?**
   - Quali categorie si sono rivelate più facili/difficili da sfruttare?

2. **Che differenze avete notato tra modelli open-source e modelli avanzati?**
   - I modelli avanzati hanno fallito nelle stesse aree?
   - Ci sono state sorprese nei risultati?

3. **Cosa abbiamo imparato sui modi corretti di interrogare gli LLM?**
   - Quali strategie di formulazione funzionano meglio?
   - Come possiamo verificare l'affidabilità delle risposte?
   - Quando è appropriato fidarsi di un LLM e quando serve verificare?

4. **Come possiamo applicare queste conoscenze nel lavoro quotidiano?**
   - Best practices per l'utilizzo professionale degli LLM
   - Come strutturare prompt per compiti complessi
   - Quando utilizzare strumenti complementari (calcolatrici, database, ricerca web)

**Tempo**: 20-30 minuti
