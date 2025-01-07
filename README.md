# Customer-Acquisition-Optimization-in-Banking
The project optimizes a bank’s marketing campaigns using predictive models (Random Forest, MLP) and evaluates performance with metrics like accuracy and AUC. Correlations between customer data and term deposit subscriptions are analyzed, with results presented in a final report.



# Previsione della Sottoscrizione a Depositi a Termine

Questo progetto di machine learning mira a prevedere se un cliente di una banca sottoscriverà o meno un deposito a termine. Il modello sviluppato può aiutare la banca a ottimizzare le proprie campagne di marketing, concentrando gli sforzi sui clienti più propensi alla sottoscrizione.

## Dati e Analisi

Il dataset utilizzato per questo progetto contiene informazioni sui clienti, tra cui:

* Dati demografici: età, professione, stato civile, livello di istruzione.
* Situazione finanziaria: presenza di insolvenze, mutuo per la casa, prestito personale.
* Dettagli sull'ultimo contatto durante la campagna di marketing: tipo di contatto, mese, giorno della settimana, durata.

Sono state eseguite analisi esplorative dei dati per identificare le variabili più rilevanti per la previsione. Sono state utilizzate diverse tecniche, tra cui:

* **Analisi della correlazione:** per valutare la forza e la direzione del legame tra variabili numeriche e target binario.
* **Test di Chi-quadro:** per valutare l'associazione statistica tra le variabili categoriali e il target.
* **Visualizzazioni grafiche:** per rappresentare le relazioni tra le variabili e il target.

## Modelli Predittivi

Sono stati addestrati e valutati diversi modelli di machine learning, tra cui:

* **Random Forest:** un modello di ensemble learning che combina diversi alberi decisionali.
* **MLP (Multi-Layer Perceptron):** una rete neurale con più layer nascosti.

## Valutazione del Modello

Le prestazioni dei modelli sono state valutate utilizzando diverse metriche, tra cui:

* **Accuratezza:** la percentuale di previsioni corrette.
* **Precisione:** la percentuale di veri positivi tra le istanze classificate come positive.
* **Richiamo (Recall):** la percentuale di veri positivi identificati rispetto al totale dei positivi reali.
* **F1 Score:** la media armonica tra precisione e richiamo.
* **AUC (Area Under Curve):** una misura della capacità del modello di discriminare tra le due classi.

## Risultati

I modelli addestrati hanno ottenuto buoni risultati in termini di accuratezza, AUC e altre metriche di valutazione. L'analisi dell'importanza delle feature ha rivelato che le variabili più influenti per la previsione sono:

* Saldo del conto (`balance`).
* Numero della settimana nell'anno (`week_number`).
* Tipo di lavoro (`job`).
* Numero di contatti durante la campagna (`campaign`).
* Mese del contatto (`month`).
* Presenza di mutuo (`housing`).
* Numero di giorni trascorsi dall'ultimo contatto (`pdays`).
* Esito della campagna precedente (`poutcome`).

## Conclusioni

Questo progetto dimostra come l'apprendimento automatico possa essere utilizzato per prevedere la sottoscrizione a depositi a termine. Il modello sviluppato può fornire alla banca informazioni utili per migliorare le proprie campagne di marketing e aumentare la redditività.

## Istruzioni per l'Uso

* Il codice del progetto è disponibile in questo repository GitHub.
* Per eseguire il codice, è necessario installare le librerie Python elencate nel file `requirements.txt`.
* Il dataset utilizzato per il training e la valutazione del modello è disponibile nella cartella `data`.
* I file `notebook` contengono il codice utilizzato per l'analisi dei dati, il training e la valutazione dei modelli.
* Il file `models` contiene i modelli addestrati.

## Possibili Miglioramenti

* Sperimentare con altri modelli di machine learning, come ad esempio XGBoost o LightGBM.
* Ottimizzare ulteriormente gli iperparametri dei modelli.
* Utilizzare tecniche di feature engineering più avanzate.
* Implementare un'interfaccia utente per rendere il modello più accessibile.
