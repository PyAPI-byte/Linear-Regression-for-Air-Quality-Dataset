# Linear-Regression-for-Air-Quality-Dataset
Questo repository contiene uno script Python sviluppato come progetto pratico per l'apprendimento dei concetti fondamentali di Machine Learning e Data Science, ispirato alla metodologia e alle best practices del celebre testo Hands-On Machine Learning with Scikit-Learn and PyTorch di Aurélien Géron.
Panoramica del Progetto
L'obiettivo principale del progetto è analizzare un dataset sulla qualità dell'aria (air_quality_dataset.csv) e costruire un modello predittivo basato su Regressione Lineare per stimare il livello di particolato PM10 partendo dai livelli di metano (CH4).

Architettura e Flusso di Lavoro
Il codice è strutturato in modo modulare seguendo due macro-fasi logiche:

Exploratory Data Analysis (EDA):

Caricamento e ispezione preliminare del dataset tramite Pandas (df.head(), df.info()).

Analisi delle correlazioni statistiche tra le variabili (df.corr()) per individuare i legami più forti con il particolato.

Generazione di grafici esplorativi e matrici di dispersione (scatter_matrix) per visualizzare la distribuzione e la relazione tra gli inquinanti.

Machine Learning Modeling & Pipeline:

Train/Test Split: Divisione casuale e riproducibile dei dati (80% training, 20% test) tramite train_test_split con seed controllato (random_state=42) per prevenire l'overfitting.

Pipeline di Preprocessing: Integrazione automatica di un SimpleImputer (strategia basata sulla mediana) per gestire eventuali valori mancanti in modo sicuro, evitando il data leakage.

Addestramento e Predizione: Fitting del modello di LinearRegression sul set di addestramento e predizioni sul set di test.

Valutazione: Calcolo dell'errore tramite la metrica RMSE (Root Mean Square Error) per quantificare la precisione delle stime.

Visualizzazione dei Risultati:

Generazione di un grafico finale in matplotlib che unisce i punti reali di training e test (con codice colore differenziato) e la retta di regressione lineare ottimizzata sull'intero intervallo dei dati.

Un progetto ideale per chi muove i primi passi nel mondo del Machine Learning, mostrando come combinare pulizia dei dati, pipeline di Scikit-Learn e visualizzazione grafica in un unico flusso pulito e professionale.
