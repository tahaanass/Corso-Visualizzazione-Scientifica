# Decodificare il Successo su Spotify 
**Progetto per il corso di Visualizzazione Scientifica**

**Autori:**
* Taha Anass Seddik
* Daniele Zmarandache

## Descrizione del Progetto
Questo studio analizza un campione massivo di oltre 100.000 tracce musicali per identificare l'identità acustica delle hit di successo. Attraverso tecniche di Exploratory Data Analysis (EDA) e l'addestramento di un modello predittivo di Machine Learning (Random Forest), il progetto mappa le combinazioni acustiche preferite dal pubblico e dagli algoritmi di raccomandazione.

L'intera analisi visiva è stata progettata con un approccio minimalista, volto a ridurre il rumore grafico e a massimizzare la chiarezza dei dati, convertendo risultati statistici complessi in raccomandazioni ingegneristiche per artisti emergenti.

## Provenienza dei Dati
Il dataset utilizzato è lo **Spotify Tracks Dataset** (composto da 114.000 brani divisi in 125 generi musicali). 
Per mantenere il repository ottimizzato e garantire la massima riproducibilità, i dati grezzi non sono salvati fisicamente in cartelle locali. Il nostro Jupyter Notebook estrae il database dinamicamente in fase di esecuzione tramite l'API di Hugging Face:
`hf://datasets/maharshipandya/spotify-tracks-dataset/dataset.csv`

## Tecnologie e Strumenti Utilizzati
L'intera pipeline di calcolo e visualizzazione è stata sviluppata in ambiente Python, sfruttando le seguenti librerie:
* **Pandas & NumPy:** Per l'importazione, la pulizia dei dati, la gestione dei valori mancanti e il *Data Wrangling* numerico.
* **Matplotlib, Seaborn & Plotly:** Per la generazione di grafici statistici statici e subplots interattivi (Violin Plot, Density Plot, Scatter Plot multivariati) ottimizzati per l'Information Design.
* **Scikit-Learn:** Per l'addestramento e il test (train_test_split) del modello di Machine Learning ad alberi decisionali (Random Forest Classifier/Regressor).
* **SciPy:** Per il calcolo statistico avanzato (es. stima della densità Kernel con `gaussian_kde`).
* **Warnings:** Per la soppressione degli avvisi di sistema, garantendo un output del notebook pulito e privo di *visual clutter*.

## Struttura del Repository
* 📁 **`Notebooks/`**: Contiene il Jupyter Notebook (`.ipynb`) con l'intero script Python (Data cleaning, EDA e Machine Learning).
* 📁 **`Images/`**: Contiene i grafici statistici definitivi esportati in alta risoluzione.
* 📄 **`Presentation.pdf` / `.pptx`**: La presentazione finale del progetto.

## Come riprodurre l'analisi
1. Clonare il repository: `git clone https://github.com/tahaanass/Corso-Visualizzazione-Scientifica.git`
2. Assicurarsi di avere un ambiente Python configurato con le librerie indicate nella sezione Tecnologie (installabili tramite `pip`).
3. Aprire il file nella cartella `Notebooks` ed eseguire tutte le celle (*Restart & Run All*). I dati verranno scaricati automaticamente.
