# SKILL_CHAT – Skill per chat con LLM

In questa cartella raccolgo le skill pronte all’uso per chat con Claude (e altri LLM).  
Ogni file definisce una singola skill, con istruzioni e contesto già ottimizzati.

## Come usare queste skill

1. Apri il file della skill che ti interessa.
2. Copia il contenuto nelle istruzioni di sistema / prompt avanzato del modello.
3. Adatta, se necessario, alcuni dettagli (lingua, tono, contesto d’uso).

---

## Elenco delle skill

### 1. historical-city-drone.skill

- **Scopo**: generare descrizioni di città storiche come se fossero viste da un drone, con taglio narrativo e divulgativo.
- **Uso tipico**:  
  - script per video social,  
  - introduzioni per articoli o newsletter,  
  - testi per voice-over di walkthrough urbani.
- **Input consigliato**: nome della città, periodo storico di interesse, eventuale focus (arte, architettura, vita quotidiana).

### 2. youtube-summarizer.skill

- **Scopo**: generare documenti strutturati a partire da video YouTube in lingua inglese.
- **Uso tipico**: report, manualistica, approfondimenti, supporto didattico e sintesi in lingua italiana.
- **Input consigliato**: basta richiamare la skill e incollare il link al video.
- **Esempio di output**: [Apri l’esempio](./youtube-summarizer-example.md)

---

## Struttura dei file di skill

Ogni file `.skill` contiene:

- Una sezione di **contesto/ruolo** (chi è il modello, come deve comportarsi).
- Le **istruzioni operative** (cosa fare, cosa evitare).
- Eventuali **esempi** di input/output.

Questo formato è pensato per essere leggibile e facilmente riutilizzabile nei vari LLM.
