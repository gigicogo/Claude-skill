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

---

## 📄 Licenza e riuso

Puoi usare, copiare, modificare e condividere questo progetto, anche per attività formative, professionali e commerciali, senza chiedere un’autorizzazione preventiva.

Salvo diversa indicazione, il codice è distribuito con licenza [MIT](https://opensource.org/license/mit), mentre i testi e i materiali didattici sono distribuiti con licenza [Creative Commons Attribuzione 4.0 Internazionale](https://creativecommons.org/licenses/by/4.0/deed.it).

Nel riuso, conserva gli avvisi previsti dalla licenza MIT; per testi e materiali didattici, cita **Gianluigi Cogo**, inserisci un collegamento al progetto originale e alla licenza e indica eventuali modifiche. Gli eventuali materiali di terzi mantengono le rispettive licenze.

## 👤 Autore e contesto

**Gianluigi Cogo** — Content creator e technical writer interessato ad AI generativa, automazioni, viaggi e strumenti digitali. Consulente e docente sui temi dell’IA generativa, dell’innovazione e della comunicazione.

- 📮 Newsletter: [gigicogo.substack.com](https://gigicogo.substack.com)
- 📝 Blog: [medium.com/webeconoscenza](https://medium.com/webeconoscenza)
- ▶️ YouTube: [youtube.com/@gigicogo](https://www.youtube.com/@gigicogo)
- 💼 LinkedIn: [linkedin.com/in/gigicogo](https://it.linkedin.com/in/gigicogo)
