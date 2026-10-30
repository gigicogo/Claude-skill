# 🏛️ AI-PA — Skill Claude per la Pubblica Amministrazione

**AI-PA** è una raccolta di skill per Claude pensate per supportare alcune attività ricorrenti della Pubblica Amministrazione: controllo formale di atti, preparazione di FAQ, sintesi di circolari, report da dati, semplificazione linguistica e verifica di coerenza.

Le skill non sostituiscono le procedure, le autorizzazioni né le valutazioni degli uffici: producono **bozze di supporto**, sempre da verificare dalla persona competente.

## 🎯 A chi è rivolto

La raccolta è pensata per:

- funzionari ed esecutori della Pubblica Amministrazione;
- uffici che preparano comunicazioni, FAQ, sintesi e report;
- direttori e dirigenti coinvolti nella governance dell’IA;
- formatori e docenti che vogliono mostrare un uso responsabile dell’AI generativa;
- chi vuole sperimentare prompt strutturati con regole chiare di tracciabilità e verifica.

## 🧠 Principio guida

Ogni skill lavora **esclusivamente sui documenti forniti dall’utente** per il caso in corso.

Non effettua ricerche esterne, non inventa norme, prassi, referenti, date, importi, contatti o collegamenti. Se un’informazione non è presente nelle fonti, la segnala come `NON PRESENTE NELLE FONTI`; se è ambigua o richiede una valutazione, la segnala come `DA VERIFICARE`.

L’obiettivo è usare l’AI come assistente alla redazione e al controllo, non come decisore amministrativo.

## 🧩 Skill disponibili

| Skill | A cosa serve | Output principale |
|---|---|---|
| [`checklist-atto`](checklist-atto.md) | Confronta una bozza di atto con un modello o schema fornito, segnalando campi presenti, mancanti, incompleti o da valutare. | Tabella di controllo formale preliminare e punti da completare |
| [`preparazione-faq`](preparazione-faq.md) | Trasforma una scheda di servizio, circolare o testo ufficiale in una prima bozza di FAQ basate solo sulle informazioni documentate. | FAQ numerate con riferimento alla fonte |
| [`report-da-dati`](report-da-dati.md) | Trasforma una tabella già verificata in un report descrittivo, separando dati, calcoli e interpretazioni. | Report descrittivo con indicatori, calcoli e limiti dei dati |
| [`semplificazione-linguistica`](semplificazione-linguistica.md) | Riscrive un testo amministrativo in italiano più chiaro, preservando condizioni, scadenze e significato. | Bozza di testo semplificato con punti da chiarire |
| [`sintesi-circolare`](sintesi-circolare.md) | Converte una circolare o comunicazione organizzativa in una scheda operativa con obblighi, scadenze e verifiche. | Sintesi operativa con destinatari, termini e controlli |
| [`verifica-coerenza`](verifica-coerenza.md) | Confronta una bozza con il documento fonte per individuare contraddizioni, omissioni o informazioni non supportate. | Tabella di segnalazioni di coerenza |

## 📄 Come sono strutturate le skill

Ogni file Markdown contiene:

- **Nome e descrizione**: quando attivare la skill.
- **Scopo**: il risultato che la skill deve produrre.
- **Input da richiedere**: documenti e informazioni necessarie.
- **Procedura**: i passaggi operativi da seguire.
- **Output richiesto**: struttura della bozza generata.
- **Regole comuni**: limiti, cautele e obblighi di verifica.

## 🔒 Regole comuni

Tutte le skill condividono le stesse regole di sicurezza e tracciabilità:

- Lavorano solo sui documenti forniti per il caso in corso.
- Non fanno ricerche esterne né introducono contenuti non documentati.
- Non accedono a sistemi esterni, non inviano comunicazioni e non modificano dati.
- Producono soltanto bozze di supporto.
- Segnalano le informazioni mancanti con `NON PRESENTE NELLE FONTI`.
- Segnalano le ambiguità con `DA VERIFICARE`.
- Indicano, quando possibile, il punto della fonte a sostegno delle informazioni.
- Non trattano dati personali reali: gli esempi sono inventati.
- Non dichiarano mai un testo conforme, approvato o pronto per la firma.

## 🚀 Come usarle

1. Apri Claude e carica o incolla il documento di lavoro necessario.
2. Scegli la skill più adatta al compito.
3. Fornisci gli input richiesti: fonte, bozza, tabella, destinatario o finalità operativa.
4. Leggi l’output come **bozza**, non come documento definitivo.
5. Verifica ogni informazione rispetto al documento originale.
6. Fai completare o validare il testo dalle persone competenti prima dell’uso.

## ✅ Regola pratica

Nessun output generato da queste skill deve essere pubblicato, firmato o considerato definitivo senza verifica umana.

In particolare:

- non pubblicare FAQ prima della validazione dell’ufficio;
- non considerare un report una valutazione o decisione amministrativa;
- non trattare una semplificazione linguistica come una nuova decisione;
- non usare una sintesi di circolare al posto del testo originale;
- non considerare la verifica di coerenza una certificazione di correttezza.

## 🧪 Possibili evoluzioni

- Aggiunta di nuove skill per comunicazioni al cittadino, verbali, questionari e risposte a istanze.
- Creazione di esempi completi per ogni skill.
- Versione inglese delle istruzioni.
- Integrazione con checklist organizzative e moduli di verifica.
- Raccolta di casi d’uso reali, resi anonimi, per l’aggiornamento delle skill.

## 🤝 Contribuire

Sono benvenuti suggerimenti su nuove skill, miglioramenti delle istruzioni, esempi didattici e correzioni.

1. Apri una Issue per proporre una nuova skill o una modifica.
2. Oppure apri una Pull Request con il file Markdown proposto.
3. Mantieni la struttura comune: scopo, input, procedura, output e regole di sicurezza.

---

## 📄 Licenza

Da definire: si suggerisce una licenza aperta (es. MIT o CC BY 4.0) per favorire il riuso da parte di altri formatori o altri enti. Sostituisci questo paragrafo con il testo della licenza scelta e il file `LICENSE` del repo.

## 👤 Autore e contesto

**Gianluigi Cogo**  
Content creator e technical writer interessato ad AI generativa, automazioni, viaggi e strumenti digitali. Consulente e docente sui temi dell’IA generativa nella Pubblica Amministrazione.

L’app nasce come esercitazione nel percorso operativo **“L’IA nella Pubblica Amministrazione — Percorso operativo per l’uso consapevole, sicuro e governato dell’IA generativa”** (20 ore: percorso base per funzionari ed esecutori + modulo governance per direttori e dirigenti). Per info sul corso contattami usando i social qui sotto.

- 📮 **Newsletter:** [gigicogo.substack.com](https://gigicogo.substack.com)
- 📝 **Blog:** [medium.com/webeconoscenza](https://medium.com/webeconoscenza)
- ▶️ **YouTube:** [youtube.com/@gigicogo](https://youtube.com/@gigicogo)
- 💼 **LinkedIn:** [linkedin.com/in/gigicogo](https://www.linkedin.com/in/gigicogo)
