# 🧩 Claude-skill — Raccolta di skill per uso didattico

**Claude-skill** è una raccolta di skill, prompt strutturati e materiali didattici per creare e usare skill su Claude e, in molti casi, anche su altri LLM compatibili.

Il repository è pensato come supporto pratico per progettare workflow conversazionali, “mini-tool” riutilizzabili e attività formative basate sull’AI generativa.

## 🎯 A chi è utile

- Creator, docenti e comunicatori che vogliono usare gli LLM in modo strutturato, non solo con prompt “al volo”.
- Chi sta imparando a progettare skill riutilizzabili per content creation, formazione o consulenza.
- Formatori e consulenti che necessitano di esempi pronti da adattare a contesti diversi.
- Dipendenti e responsabili della Pubblica Amministrazione interessati a un uso consapevole dell’IA generativa.

## 🗂️ Struttura del repository

| Cartella | Contenuto | Stato |
|---|---|---|
| [`AI-PA/`](AI-PA/) | Skill pronte all’uso per compiti specifici della Pubblica Amministrazione. | ✅ Popolata |
| [`MANUAL_CHAT/`](MANUAL_CHAT/) | Skill e materiali per creare skill manualmente, passo dopo passo, senza assistenti automatici. | 🚧 In preparazione |
| [`SKILL_CHAT/`](SKILL_CHAT/) | Skill pronte all’uso per la chat: descrizioni di città, contenuti per video, testi divulgativi e altro. | 🚧 In preparazione |

Alcune cartelle sono ancora in costruzione: la struttura è già definita, ma i file e gli esempi verranno aggiunti progressivamente.

## 🏛️ AI-PA

La cartella [`AI-PA/`](AI-PA/) raccoglie skill utilizzate soprattutto nei percorsi formativi per la Pubblica Amministrazione.

Ogni skill lavora sui documenti forniti dall’utente, produce una bozza di supporto e richiede sempre la verifica della persona competente.

| # | Skill | Caso d’uso |
|---:|---|---|
| 1 | [`sintesi-circolare`](AI-PA/sintesi-circolare.md) | Sintesi operativa di una circolare fittizia per uno sportello |
| 2 | [`semplificazione-linguistica`](AI-PA/semplificazione-linguistica.md) | Riscrittura di un avviso scritto in burocratese |
| 3 | [`checklist-atto`](AI-PA/checklist-atto.md) | Controllo formale di una bozza di determinazione rispetto a uno schema |
| 4 | [`verifica-coerenza`](AI-PA/verifica-coerenza.md) | Confronto tra una circolare e una sintesi o bozza derivata |
| 5 | [`preparazione-faq`](AI-PA/preparazione-faq.md) | Preparazione di FAQ a partire da una circolare |
| 6 | [`report-da-dati`](AI-PA/report-da-dati.md) | Report descrittivo da un CSV con dati fittizi e metriche verificabili |

👉 Consulta la documentazione completa nella cartella [`AI-PA/`](AI-PA/README.md).

## 🛠️ MANUAL_CHAT

La cartella `MANUAL_CHAT/` sarà dedicata alla creazione **manuale** delle skill.

Sarà utile per capire:

- la logica alla base di una skill;
- come definire scopo, input, procedura e output;
- come scrivere istruzioni chiare e ripetibili;
- come costruire una skill da zero, senza assistenti automatici.

## 💬 SKILL_CHAT

La cartella `SKILL_CHAT/` raccoglierà skill pronte all’uso per la chat.

Gli esempi previsti includono:

- descrizioni di città e destinazioni;
- contenuti per video e social;
- testi divulgativi;
- materiali per la comunicazione e la formazione.

Ogni file rappresenterà una singola skill. Il README della cartella spiegherà come usarle e, dove disponibile, collegherà esempi di output.

## 🚀 Come usare queste risorse

1. Scegli la cartella più adatta al tuo obiettivo: `AI-PA`, `MANUAL_CHAT` o `SKILL_CHAT`.
2. Apri i file `.md` per leggere spiegazioni, istruzioni e contesto d’uso.
3. Consulta i file `.skill`, dove presenti, per vedere la struttura operativa.
4. Se disponibile, esamina gli esempi di output per capire il risultato atteso.
5. Copia e adatta le skill nel tuo ambiente di lavoro con Claude o altri LLM compatibili.

## 🧪 Sviluppi futuri

Il repository potrà accogliere:

- nuove sezioni tematiche;
- integrazioni con API;
- esempi per altri modelli e piattaforme;
- template riutilizzabili per formazione e consulenza;
- casi d’uso completi, con input, skill e output di esempio.

## 🤝 Contribuire

Sono benvenuti suggerimenti, nuove skill, esempi didattici, correzioni e materiali di supporto.

1. Apri una Issue per proporre un’idea o segnalare un problema.
2. Oppure apri una Pull Request con una nuova skill o una modifica.
3. Mantieni una struttura chiara: scopo, input, procedura, output e regole d’uso.

---

## Contesto del progetto

Il repository nasce come supporto al percorso operativo **“L’IA nella Pubblica Amministrazione — Percorso operativo per l’uso consapevole, sicuro e governato dell’IA generativa”** (20 ore: percorso base per funzionari ed esecutori + modulo governance per direttori e dirigenti).

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
