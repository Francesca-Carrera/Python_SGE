# Progetto Python – Sistema di Gestione Elementi (SGE) per il media brand "Voci".

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

**File principale:** `FrancescaCarrera_Python.ipynb`

**Obiettivo del progetto**  
Un media brand chiamato "Voci", nato per riequilibrare la narrazione mediatica spesso dominata da prospettive maschili, aveva bisogno di uno strumento strutturato per organizzare e analizzare i contenuti pubblicati (testimonianze, approfondimenti, atti di attivismo).  

Questo progetto sviluppa un **Sistema di Gestione degli Elementi (SGE)** che consente agli utenti di:
- Effettuare ricerche selezionando uno o più criteri (categoria, posizionamento, narrativa, parola nei titoli).
- Visualizzare l'intero dataset, scegliendo l'ordinamento principale (per categoria, per narrativa, per posizionamento crescente).
- Consultare insight e analisi statistiche (conteggio totale, top/bottom 5, parole più frequenti nei titoli, distribuzione percentuale per narrativa, posizionamento medio per categoria/narrativa, categorie/narrative nei primi 10 posizionamenti).
- Registrare nuovi contenuti, organizzandoli tematicamente con validazione avanzata del titolo.

**Strumenti e librerie utilizzate**  
- **Python 3** – linguaggio di programmazione.
- **Jupyter Notebook** – ambiente di sviluppo interattivo.
- `rich.console` e `rich.table` – visualizzazione tabellare avanzata e formattazione della console.
- `string` – operazioni su caratteri e punteggiatura per la validazione dei titoli.
- `time` – sincronizzazione dell'output per una migliore esperienza utente.

**Struttura del progetto**  
Il progetto è contenuto in un unico file Jupyter Notebook (`FrancescaCarrera_Python.ipynb`), strutturato in sezioni logiche:

1. **Configurazione iniziale** – dataset `gender_media_dataset_voci` (dizionario con 11 categorie tematiche e oltre 40 articoli), importazioni, costanti simboliche.
2. **Classi Model** – logica dei dati e operazioni tematiche (ricerca singola e multipla, visualizzazione, registrazione, analisi).
3. **Classi View** – interfaccia utente testuale (menu, istruzioni, feedback).
4. **Classi Controller** – flusso di controllo, navigazione, coordinamento Model-View (pattern MVC).
5. **Punto d'ingresso** – avvio interattivo dell'applicazione.
6. **Scenario Testing** – funzione `esegui_scenario()` per test automatizzati con input simulati.

**Architettura**  
Il codice segue un'architettura ispirata al pattern **MVC (Model-View-Controller)**. La classe `HomeController` funge da punto di ingresso unico (pattern Facade), semplificando l'accesso a tutte le funzionalità. L'intero sistema è sviluppato in Python puro.

**Gestione degli errori**  
- Il dataset di partenza (`gender_media_dataset_voci`) è considerato strutturalmente valido (non vengono sollevate eccezioni sulla sua struttura).
- La registrazione di nuovi articoli avviene in modo controllato con validazione avanzata.

**📌 **Feedback del tutor (Start2Impact)**  

> *"Ho visionato il tuo progetto e hai fatto un ottimo lavoro: credo sia tra i progetti più completi e complessi mai ricevuti! Complimenti."*  
> *"Sono davvero impressionato dell’impegno che hai dimostrato. Vedo un grande potenziale in te."*  
> *"Le aziende apprezzano molto i progetti ben documentati e curati nei dettagli. Per questo ti faccio i miei complimenti: il risultato che hai raggiunto è buono."*  
> *"Ottimo anche l’uso di esempi di esecuzione estensivi, che permettono di valorizzare al meglio il lavoro svolto."*  
> *"ottimo lavoro!"*  

> — *Andrea, Lead AI Engineer in Lundbeck – Start2Impact*

**Repository:** [github.com/Francesca-Carrera/Python_Voci_SGE](https://github.com/Francesca-Carrera/Python_Voci_SGE)
