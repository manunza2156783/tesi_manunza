# Tesi triennale AI e Ambiente - Simone Manunza (2156783)

La repository contiene tutti gli script e i dataset utilizzati per la tesi triennale "AI e Ambiente" per il corso di Laurea in Filosofia e Intelligenza Artificiale (2025-2026) alla Sapienza Università di Roma, per il laureando Simone Manunza (2156783) con Relatrice Prof.ssa Flavia Monti e Correlatrice Dott.ssa Elisabetta Arba. 

---
# Abstract
Il progetto pratico ha come fine quello di analizzare il trade-off tra l'utilizzo del ML per predire gli indici di inquinamento e le stesse emissioni dovute al consumo di energia per l'addestramento di tali modelli. I dati utilizzati provengono da: IDEAH, un progetto dell'ISS, che ha fornito i rilevamenti di agenti inquinanti con copertura di un mese (dal 14 giugno al 14 luglio); e da API open source come OpenMeteo e OpenAQ, per integrare i restanti undici mesi di rilevamenti inquinanti e di condizioni climatiche. Una volta addestrati i modelli i loro conseguenti consumi ed emissioni sono stati calcolati utilizzando il tool open source Green Algorithms.
Precisamente gli agenti inquinanti presi in analisi sono: NO₂, O₃, SO₂, CO, PM10, PM2.5. Questi sono stati predetti con i seguenti modelli: XGBoost, LightGBM, SGDRegressor, Random Forest, Decision Trees.

---
# Istruzioni

Tutti i dataset utilizzati si trovano nella cartella "dataset" e sono stati caricati con l'utilizzo di Git Large File Storage. Qui si trovano tutte le versioni dei dataset, a partire da quella iniziale, "dati_tesi_incompleti.csv", cioè i dati scaricati dal server IDEAH, con poi tutte le versioni intermedie in cui sono stati scaricati i dati tramite utilizzo API di OpenMeteo e OpenAQ, fino ad arrivare alla versione finale, "dati_tesi_finali_addestramento.csv"

Nella cartella "dati rilevamenti agenti" si trova lo script per il download dei dati da OpenAQ, mentre nella cartella "dati condizioni climatiche" si trova lo script per il controllo delle stazioni offerte da OpenMeteo, in quanto i dati da questa fonte sono stati scaricati direttamente dal sito e non tramite script Python con limite di delta per la distanza tra la stazione offerta e quella originale di riferimento.

Si trova, poi, l'EDA sul dataset finale, creato con gli script delle cartelle precedentemente nominate, e, infine, l'addestramento dei modelli.