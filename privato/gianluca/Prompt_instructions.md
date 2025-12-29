# Istruzioni

## 1 Evitare ambiguità

Il prompt deve essere **chiaro e preciso**, altrimenti l’AI può fraintendere e dare una risposta sbagliata, incompleta o diversa da quella che ci aspettavamo.
Alcune parole possono avere più significati e se non specifichiamo cosa intendiamo, l’AI deve “indovinare”.
Più dettagli diamo (argomento, contesto, tipo di risposta), migliore sarà il risultato.

**Esempio di prompt ambiguo:**
``` 
- Prompt vago:  “Scrivi una poesia.”

- Prompt preciso: “Scrivi una poesia breve in rima sulla primavera.”
```
```
- Prompt vago:  “Aiutami a fare una ricerca sulla rete”

- Prompt preciso: “Aiutami a fare una ricerca sulla rete internet e la sua storia”
```


## 2 Essere concisi

Essere e dire solo ciò che serve, usando un linguaggio chiaro. Frasi troppo elaborate, richieste eccessivamente dettagliate o l’uso di termini inutilmente complessi rendono più difficile per l’AI capire qual è l’obiettivo principale della richiesta.

Un altro problema comune è quando in un unico prompt si mescolano **troppe domande o argomenti diversi**. In questi casi l’AI può rispondere in modo confuso o incompleto. È spesso meglio dividere una richiesta complessa in più prompt semplici, ciascuno con un obiettivo chiaro.

```
Prompt con vocaboli superflui:

- Ti sarei molto grato se potessi fornirmi una spiegazione completa del processo metabolico.

Prompt immediato:

- Spiegami il metabolismo umano.
```


```
Prompt con troppi argomenti insieme:

- “Spiega gli effetti del cambiamento climatico sull’agricoltura, le risposte politiche e il ruolo futuro dell’intelligenza artificiale nella sicurezza alimentare.”

Prompt divisi e più chiari:

- “Quali sono gli effetti del cambiamento climatico sull’agricoltura?”

- “Come stanno rispondendo i governi a questi problemi?”

- “In che modo l’AI potrebbe aiutare a combattere l’insicurezza alimentare?”
```

## 3 Specificare senza esagerare

Essere specifici aiuta l’AI a capire chiaramente cosa deve fare e su quale argomento concentrarsi. Tuttavia, fornire troppi dettagli può risultare controproducente: il modello può confondersi o produrre una risposta frammentata e poco coerente.

Essere specifici significa indicare chiaramente:

- l’obiettivo della richiesta

- il contesto

- l’aspetto principale su cui concentrarsi

Evitare l’over-specificazione significa non trasformare il prompt in una lista eccessiva di vincoli, dati e sotto-compiti che limitano la capacità dell’AI di organizzare una risposta efficace o creativa.

```
Prompt eccessivamente specifico:

“Riassumi il paper sul cambiamento climatico e gli orsi polari includendo dati su temperature, scioglimento dei ghiacci, migrazioni, tassi di natalità, mortalità e confronti con gli ultimi 50 anni.”

Prompt bilanciato:

“Riassumi il paper sul cambiamento climatico e gli orsi polari concentrandoti sull’habitat e sull’andamento della popolazione.”
```


## 4 Includere il contesto 

Dare all’AI le informazioni di base necessarie per capire meglio la situazione e l’obiettivo della richiesta. Il contesto aiuta il modello a interpretare correttamente l’intento dell’utente e a produrre risposte più precise e adatte al caso specifico.

Senza contesto, l’AI può dare risposte corrette ma generiche, oppure interpretare male la richiesta.

Il contesto può riguardare:

- l’argomento specifico

- il livello di conoscenza dell’utente

- il ruolo o la situazione dell’utente

- il pubblico a cui è destinata la risposta

- lo scopo della richiesta

```

Prompt generico:

“Dammi consigli per essere più produttivo.”

Prompt con contesto:

“Dammi consigli per migliorare la produttività di uno studente universitario durante la sessione d’esami.”
```
```

Prompt senza indicazione del pubblico:

“Spiega l’effetto serra.”

Prompt con contesto sul pubblico:

“Spiega l’effetto serra a un bambino di 8 anni.”
```

## 5 Fornire esempi

Aiuta l’AI a capire che tipo di risposta ci aspettiamo. Gli esempi funzionano come un **modello da imitare**: 
- mostrano il formato
- il tono
- il livello di dettaglio
- lo stile desiderato




Poiché l’AI è molto brava a riconoscere schemi, più esempi riceve, meglio riesce ad adattare la risposta a nuove situazioni simili.

Gli esempi riducono l’ambiguità e rendono più chiaro l’obiettivo del compito. Sono utili sia in contesti creativi (scrittura, stile narrativo) sia in contesti tecnici (riassunti, spiegazioni, procedure).

```
Prompt creativo generico: 

“Scrivi una descrizione.”

Prompt con esempio di stile: 

“Ecco lo stile che voglio: ‘Il sole tramontava tingendo il cielo di rosso.’ Ora scrivi una descrizione simile di una giornata piovosa.”

```

### Attenzione

Il modello potrebbe replicare in modo troppo letterale lo stile o il formato dell’esempio.
Esempi troppo pochi o troppo specifici possono restringere artificialmente lo spazio delle risposte possibili.

L’AI potrebbe cogliere pattern non intenzionali presenti negli esempi, come lunghezza, struttura o scelte lessicali non volute.


**Quando usare gli esempi**

- Nei compiti creativi.

- Quando il formato o lo stile della risposta è fondamentale.

- Quando si vuole uniformare l’output (ad esempio molti riassunti simili).

**Quando evitarli**

- Quando si vogliono esplorare soluzioni diverse.

- Quando si cerca completezza o varietà di approcci.

- Quando si desidera lasciare massima libertà interpretativa all’AI.


## 6 Usare analogie


Spiegare o descrivere qualcosa facendolo assomigliare a qualcosa di già noto. Le analogie aiutano l’AI a cogliere meglio concetti astratti, stili o atmosfere, perché collegano l’ignoto a un riferimento familiare.

In un prompt, un’analogia fornisce un contesto implicito molto forte: suggerisce tono, emozione, struttura o caratteristiche senza doverle elencare tutte. Questo rende la richiesta più efficace e orienta la risposta in modo naturale.

Le analogie sono particolarmente utili per:

- scrittura creativa

- descrizioni

- concetti astratti o complessi

- comunicazione evocativa


```
Prompt tecnico poco evocativo:

“Descrivi un prodotto resistente.”

Prompt con analogia:

“Descrivi il prodotto come se fosse duro come un diamante.”

```

## 7 Usare verbi d’azione


Iniziare la richiesta con un verbo chiaro che indichi esattamente cosa deve fare l’AI. I verbi d’azione rendono il compito esplicito e orientano subito il tipo di risposta attesa.

Verbi diversi portano a risposte diverse:

- alcuni richiedono analisi

- altri spiegazioni

- altri ancora creatività o valutazioni

Scegliere il verbo giusto aiuta a evitare ambiguità e a ottenere risposte più pertinenti e mirate.

Alcuni esempi di verbi utili sono: 
- analizza
- confronta
- descrivi 
- spiega
- valuta
- riassumi 
- crea
- identifica 
- prevedi

```
Prompt poco diretto:

“Quali sono le differenze tra questi due sistemi?”

Prompt con verbo d’azione:

“Confronta i due sistemi evidenziando le principali differenze.”

``` 


## 8 Specificare il formato dell’output

Dire chiaramente come deve essere presentata la risposta, non solo cosa deve contenere. Indicare struttura, lunghezza, stile o tono aiuta l’AI a organizzare meglio le informazioni e a fornire un risultato immediatamente utilizzabile.

Quando il formato non è specificato, l’AI può comunque rispondere correttamente, ma in un modo che potrebbe non essere adatto allo scopo dell’utente. Definendo il formato, si riduce la necessità di correzioni successive e si rende l’interazione più efficiente.

Il formato può riguardare:

- struttura (elenco puntato, testo discorsivo, tabella)

lunghezza

- stile o tono (formale, informale, tecnico)

- tipo di contenuto (riassunto, lettera, codice, poesia)

```
Prompt senza formato:

“Riassumi le fasi del metabolismo.”

Prompt con formato specificato:

“Fornisci una elenco puntato sulle fasi del metabolismo, con una spiegazione breve per ogni punto.”

```


## 9 Incorporare conoscenza 

Incorporare la conoscenza di dominio significa usare terminologia e concetti specifici di un settore all’interno del prompt. Questo aiuta l’AI a capire il livello di competenza richiesto e a fornire risposte più accurate.

L’uso di termini tecnici riduce l’ambiguità e segnala all’AI che la risposta deve essere contestualizzata in un ambito specifico. In questo modo, l’output sarà più mirato e utile per chi opera in quel settore.

```
Prompt legale poco preciso:

“Quali sono le pene per frode?”

Prompt con contesto giuridico:

“Quali sono le pene per frode secondo il Fraud Act del 2006 nel Regno Unito?”
```

## 10 Evitare domande tendenziose

Fare domande dirette significa porre quesiti neutri e chiari, senza suggerire una risposta implicita. Le domande dirette aiutano l’AI a fornire risposte più **obiettive e affidabili**.

Le domande tendenziose (leading questions), invece spingono l’AI verso una risposta predefinita, introducendo bias e riducendo la qualità dell’informazione ottenuta.

Le domande dirette sono particolarmente importanti quando si cercano:

- valutazioni imparziali

- confronti equilibrati

- analisi di temi complessi

```
Domanda diretta:

“Quali sono i benefici del lavoro da remoto?”

Domanda tendenziosa:

“Perché il lavoro da remoto è più produttivo?”
``` 

