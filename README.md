# Tesi triennale AI e Ambiente - Simone Manunza (2156783)

La repository contiene lo script di addestramento dei modelli per la tesi triennale "AI e Ambiente" per il corso di Laurea in Filosofia e Intelligenza Artificiale (2025-2026) alla Sapienza Università di Roma, per il laureando Simone Manunza (2156783) con Relatrice Prof.ssa Flavia Monti e Correlatrice Dott.ssa Elisabetta Arba. 

---
# Spiegazione dello studio
Il progetto pratico ha come fine quello di analizzare il trade-off tra l'utilizzo del ML per predire gli indici di inquinamento e le stesse emissioni dovute al consumo di energia per l'addestramento di tali modelli. I dati utilizzati provengono da: IDEAH, un progetto dell'ISS, che ha fornito i rilevamenti di agenti inquinanti con copertura di un mese (dal 14 giugno al 14 luglio); e da API open source come OpenMeteo e OpenAQ, per integrare i restanti undici mesi di rilevamenti inquinanti e di condizioni climatiche. Una volta addestrati i modelli i loro conseguenti consumi ed emissioni sono stati calcolati utilizzando il tool Green Algorithms.

Precisamente gli agenti inquinanti presi in analisi sono:
- NO₂
- O₃
- SO₂
- CO
- PM10
- PM2.5

I livelli di quantità di presenza nell'aria di questi agenti, espressi in µg/m³, sono stati predetti con i seguenti modelli:
- eXtreme Gradient Boosting
- Light Gradient Boosting Machine
- Stochastic Gradient Descent Regressor
- Random Forest
- Decision Trees

Sono stati effettutati 3 fold stagionali: 
1. Fold 1 (test invernale):    Train: gen–set | Val: ott | Test: nov–dic
2. Fold 2 (test estivo):       Train: gen–apr | Val: mag | Test: giu–lug
3. Fold 3 (test primaverile):  Train: gen–feb | Val: mar | Test: apr–mag

A causa delle grandi varianze tra i differenti agenti, per ogni addestramento si è creato un modello singolo per ciascun agente, per ciascun fold. 

Infine, come metriche di errore si sono adottate:
- Mean Absolute Error
- Root Mean Squared Error
- R²
Ultimamente scegliendo R² come metrica principale per la valutazione dei modelli.

---
# Istruzioni
Nella repository non è presente il dataset con cui sono stati addestrati i modelli in quanto contiene dei dati distribuiti dall'ISS in maniera privata per fini di ricerca, è presente, però, lo script di addestramento dei modelli, con grafici di analisi dei risultati, e nella cartella sono presenti i singoli risultati per ogni modello.
