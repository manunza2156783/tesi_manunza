# Tesi triennale AI e Ambiente - Simone Manunza (2156783)

La repository contiene lo script di addestramento dei modelli per la tesi triennale "AI e Ambiente" per il corso di Laurea in Filosofia e Intelligenza Artificiale (2025-2026) alla Sapienza Università di Roma, per il laureando Simone Manunza (2156783) con Relatrice Prof.ssa Flavia Monti e Correlatrice Dott.ssa Elisabetta Arba. 

---
# Abstract
Il progetto pratico ha come fine quello di analizzare il trade-off tra l'utilizzo del ML per predire gli indici di inquinamento e le stesse emissioni dovute al consumo di energia per l'addestramento di tali modelli. I dati utilizzati provengono da: IDEAH, un progetto dell'ISS, che ha fornito i rilevamenti di agenti inquinanti con copertura di un mese (dal 14 giugno al 14 luglio); e da API open source come OpenMeteo e OpenAQ, per integrare i restanti undici mesi di rilevamenti inquinanti e di condizioni climatiche. Una volta addestrati i modelli i loro conseguenti consumi ed emissioni sono stati calcolati utilizzando il tool Green Algorithms.
Precisamente gli agenti inquinanti presi in analisi sono: NO₂, O₃, SO₂, CO, PM10, PM2.5. Questi sono stati predetti con i seguenti modelli: XGBoost, LightGBM, SGDRegressor, Random Forest, Decision Trees.

---
# Istruzioni

Nella repository è presente solamente lo script di addestramento dei modelli in quanto questi sono stati addestrati con dati privati, qui sono presenti i risultati dei modelli addestrati.
