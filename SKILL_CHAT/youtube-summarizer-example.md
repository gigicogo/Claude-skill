# Esempio output – youtube-summarizer.skill

## Video di partenza
Titolo: ...
Link: ...

## Obiettivo
Riassumere il contenuto in modo chiaro, sintetico e utile per un lettore non tecnico.

## Output generato
[qui incolli l’output]

## Perché è un buon esempio
- Evidenzia i concetti chiave
- Riduce la lunghezza senza perdere il senso
- Mantiene un tono leggibile e divulgativo


---

# Beyond LLM: Potenziare le Applicazioni con Large Language Models
**Corso:** CS230 Deep Learning — Stanford University | **Durata:** ~1h 49m

---

## 📌 Panoramica
Lezione pratica del corso CS230 di Stanford che accompagna gli studenti dal concetto di neurone singolo fino alla progettazione di sistemi AI agentici complessi. Il docente mappa l'intero stack di tecniche disponibili per potenziare un LLM base — dal prompting al RAG fino ai workflow multi-agente — con un orientamento esplicitamente professionale e applicativo.

---

## 🔑 Punti chiave
- I modelli LLM base hanno limitazioni strutturali: conoscenza non aggiornata, contesto limitato, difficoltà di controllo, lacune su domini specifici
- Il **prompt engineering** è la prima e più flessibile linea di ottimizzazione: zero-shot, few-shot, chain-of-thought, prompt chaining
- Il **fine-tuning** è spesso sconsigliato: costoso, lento, soggetto a overfitting e rapidamente obsoleto rispetto ai nuovi modelli
- Il **RAG** risolve i problemi di contesto, aggiornamento e sourcing integrando basi di conoscenza esterne senza toccare il modello
- I **workflow agentici** trasformano l'LLM da strumento passivo a sistema che pianifica, esegue azioni, usa tool e aggiorna la memoria
- La **valutazione (eval)** richiede metriche sia oggettive che soggettive, component-level ed end-to-end
- I sistemi **multi-agente** abilitano parallelismo, specializzazione e riuso degli agenti
- Il futuro passa per nuove architetture, multimodalità e velocità di cambiamento senza precedenti

---

## 📖 Contenuto dettagliato

### 1. Limiti dei modelli LLM base `[00:03]`
Domanda aperta agli studenti per costruire il quadro dei problemi: domain knowledge mancante, distribution shift, conoscenza non aggiornata (aneddoto su Trump e "covfefe" che mandò in crisi i sistemi Twitter nel 2017), controllabilità difficile (caso del bot Tay di Microsoft rimosso dopo 16 ore), performance insufficienti su task specializzati ad alta precisione, contesto limitato (~200K token = circa 2 libri), allucinazioni pericolose in ambiti medici ed educativi.

### 2. Prompt Engineering `[00:17]`
Zero-shot, few-shot (con esempio di classificazione recensioni biotech calibrata sul contesto aziendale), chain-of-thought, prompt chaining (esempio: email di risposta a cliente insoddisfatto spezzata in 3 prompt sequenziali con output intermedi verificabili). Introdotto il concetto di **LLM-as-judge** per valutazione automatica degli output: pairwise comparison, single answer grading, rubric-based grading con esempi few-shot.

### 3. Fine-Tuning `[00:41]`
Posizione critica esplicita del docente. Tre motivi principali: richiede molti dati etichettati, è costoso e lento, per il tempo che ci vuole esce un modello base migliore. Esempio illustrativo: fine-tuning su messaggi Slack che produce un modello che risponde "ci lavoro domani mattina" anziché eseguire il compito, imitando il comportamento umano per overfitting. Rimane valido solo per output ad alta precisione su linguaggio di dominio molto specifico.

### 4. RAG — Retrieval Augmented Generation `[00:44]`
Meccanismo base: embedding dei documenti → vector database → retrieval per distanza vettoriale → inserimento come contesto nel prompt finale. Tecniche avanzate: **chunking gerarchico** (documento + capitoli + paragrafi per migliore sourcing), **HyDE** (Hypothetical Document Embeddings: si genera un documento fittizio dalla query per migliorare la rilevanza del retrieval). Soluzione privilegiata per knowledge management, sourcing, aggiornamento continuo senza retraining.

### 5. Workflow Agentici `[00:54]`
Definizione di Andrew Ng di "agentic workflow" come alternativa al termine ambiguo "agente". Architettura: prompts + context management (working memory veloce vs archival memory lenta) + tools (API, web search, code executor) + risorse (CRM, database). Gradi di autonomia: step hardcodati → tool hardcodati step liberi → agente crea tool in autonomia. Introdotto **MCP (Model Context Protocol di Anthropic)** come standard per comunicazione agent-to-agent scalabile. Distinzione chiave tra ingegneria deterministica (sicura, prevedibile) e fuzzy engineering (flessibile ma fragile, richiede guardrail).

### 6. Eval `[01:19]`
Come misurare se un agente funziona davvero. Metriche **oggettive** (il volo prenotato è il più economico?), metriche **soggettive** (ha scelto correttamente tra volo diretto e coincidenza?), valutazione **end-to-end** (rating utente) vs **component-based** (ogni step del workflow). LLM judge con rubric per scalare la valutazione senza revisione umana continua.

### 7. Sistemi Multi-Agente `[01:34]`
Vantaggio principale: parallelismo e riusabilità degli agenti tra team diversi. Esercizio interattivo: progettazione di un sistema di home automation con agenti specializzati (clima, sicurezza, energia, frigo, meteo, orchestratore) in struttura gerarchica con connessioni dirette dove necessario via MCP.

### 8. Tendenze Future `[01:43]`
Plateau degli LLM e necessità del prossimo salto architetturale; multimodalità come fonte di guadagni trasversali; integrazione di più paradigmi di apprendimento ispirata all'apprendimento umano; velocità di cambiamento come ragione per preferire comprensione ampia a competenze tecniche specifiche (half-life delle skill molto basso).

---

## 💡 Conclusioni e Takeaway
La lezione offre una mappa pratica completa: si parte dal prompting come prima leva flessibile, si sale verso RAG e workflow agentici per gestire complessità crescente. Il messaggio centrale è evitare il fine-tuning quando possibile, investire nella valutazione sistematica, e pensare ai sistemi AI come si pensa al management. In un campo che cambia ogni sei mesi, la priorità non è padroneggiare ogni tecnica, ma costruire la capacità di capire e imparare velocemente.
