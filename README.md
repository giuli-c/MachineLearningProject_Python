# MachineLearningProject_Python
Lo scopo principale del progetto è quello di creare un modello di classificazione che sia in grado di riconoscere l'abbandono o il successo degli studenti durante il loro anno accademico.
Per fare ciò è stato analizzato un set di dati elaborato in 3 step: 
1. divisione casuale in due set di dati, dove il 70% è stato usato per generare i dati di addestramento e il 30% per i dati di test. 
2. Il set di dati di addestramento è stato ulteriormente suddiviso tramite tecnica di CROSS-VALIDATION, in modo da garantire una valutazione più accuarata del modello. 
3. Il set di dati di addestramento è stato utilizzato per ricercare il modello migliore e i parametri migliori per addestrare il modello tramite la tecnica di GRIDSEARCHCV.
I modelli utilizzati da confrontare sono stati i seguenti:
   1. LogisticRegression,
      Modello statistico usato per problemi di classificazione e analisi di predittività. Calcola la probabilità che un'istanza appartenga a una delle due classi utilizzando la funzione       
      logistica per mappare l'output lineare a una probabilità compresa tra 0 e 1.
      'max-iter' specificare il numero massimo di iterazioni (epoche) che l'algoritmo deve eseguire per ottimizzare i pesi del modello.
   2. SVC: "Support Vector Classification",
      Divide i dati in base alle 2 classi definite, cercando il miglior iperpiano (confine che esiste tra i 2).
      Perchè utilizzarlo: offre una buona precisione ed esegue previsioni più veloci rispetto all'algoritmo Naïve Bayes. Usa anche meno memoria perché usa un sottoinsieme di punti di 
      allenamento nella fase decisionale. La sua funzione principale è trovare il miglior iperpiano per separare le classi di dati: in questo caso viene utilizzato un kernel lineare. 
   3. RandomForest (MIGLIORE),
      Algoritmo che si basa su una tecnica che si chiama 'bagging'  e combina diversi alberi decisionali per migliorare le prestazioni del modello.
      Si occupa della creazione di alberi decisionali ognuno dei quali è un classificatore. Ogni albero viene addestrato su un sottoinsieme casuale dei dati di addestramento e delle 
      caratteristiche del dataset. Questo significa che ogni albero può vedere solo una parte dei dati, il che aiuta a ridurre il rischio di overfitting (sovradattamento) e aumenta la 
      diversità tra gli alberi.
