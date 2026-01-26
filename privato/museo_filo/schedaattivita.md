# Museo della filosofia 

## Intelligenza Artificiale
#### Cosa possiamo (e non possiamo) chiederle



### 1. Introduzione 

L'intelligenza artificiale generativa (ChatGPT, Gemini, Claude e tutti gli altri) sta rivoluzionando il modo con cui gestiamo la conoscenza. 

In modo estremamente semplice (usando il linguaggio naturale) abbiamo accesso a (quasi) l'intera conoscenza enciclopedica codificata dalla nostra società. 

Possiamo ottenere informazioni, organizzarle in varie forme (riassunti, tabelle, presentazioni) e anche svolgere operazioni nel web.

È quindi fondamentale imparare a conoscere questi strumenti con le loro caratteristiche, le loro potenzialità e i loro limiti.

Vi proponiamo quindi un'attività per mettere alla prova le vostre capacità di fare domande a un LLM: 

- come ottenere i risultati migliore
- come capire quanto fidarvi delle risposte 
- come migliorare i risultati ottenuti

Lo faremo attraverso attività pratiche ma prima diciamo molto velocemente come sono fatti questi strumenti di IA generativa.

I Large Language Models (LLM) sono modelli di intelligenza artificiale addestrati su enormi quantità di testo che possono generare linguaggio naturale in coerenza con alcune istruzioni. Lavorano grazie a reti neurali che possono configurarsi attraverso miliardi di parametri. La dimensione della loro "memoria" è quindi un aspetto centrale ma non è la cosa più importante. Il meccanismo fondamentale con cui apprendono si basa sul **masking**: durante l'addestramento, alcune parole vengono nascoste e il modello deve imparare a prevederle dal contesto.

**Vediamo un esempio concreto di come funziona il masking:**

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

### 2. Incominciamo con un Quiz 

Detto questo iniziamo subito a mettere alla prova le nostre competenze con un Quiz.

Per ogni quesito indicheremo due prompt diversi e vi chiederemo di indicare quale è più efficace.

Cosa è un prompt? È semplicemente l'istruzione che diamo a un'IA generativa per ottenere una risposta. In pratica, è il testo che scriviamo nella chat per comunicare con l'IA.

Il "prompt engineering" è diventato una vera e propria competenza: l'arte di formulare richieste efficaci per ottenere i migliori risultati dall'IA.

### 4\. Spingere i modelli a generare percorsi di ragionamento

Negli ultimi anni sono state sviluppate diverse strategie per impiegare i Large Language Models (LLM) in compiti che richiedono capacità di ragionamento, come la risoluzione di problemi matematici, scientifici o logici. Quando a un modello viene richiesta esclusivamente la risposta finale, senza esplicitare il processo che conduce alla soluzione, la probabilità di errore risulta spesso elevata. Numerosi studi hanno infatti mostrato che, se il modello viene guidato a produrre un ragionamento passo per passo, le risposte tendono a essere più accurate.

Questa capacità può essere potenziata dagli utenti principalmente in due modi: fornendo esempi di ragionamento oppure impartendo istruzioni esplicite su come ragionare.

L’attività di oggi si concentra su quest’ultimo aspetto. Esamineremo alcune proposte per formulare istruzioni in grado di guidare i modelli nella generazione di risposte motivate da un percorso di ragionamento e metteremo alla prova queste strategie confrontandole con prompt standard. Il confronto verrà svolto su tre domini differenti: una domanda in ambito medico, un compito di ragionamento probabilistico e un problema di fisica elementare. Analizzeremo quindi le differenze tra i risultati ottenuti e rifletteremo sulle loro implicazioni.
