---
name: checklist-atto
description: "Usa questa skill quando l’utente fornisce un modello o schema di atto amministrativo e una bozza e desidera controllare la presenza dei campi richiesti dal modello, non la conformità legale."
---

# Checklist di un atto

## Scopo
Confrontare la bozza di un atto con un modello fornito dall’utente, per segnalare sezioni e campi mancanti senza svolgere un giudizio di legittimità.

## Input da richiedere
- Modello o elenco di campi attesi dell’ente.
- Bozza dell’atto da analizzare.

## Procedura
1. Estrai dal **modello fornito** i campi richiesti, con eventuali condizioni (es. importo e capitolo se l’atto prevede una spesa).
2. Cerca nella bozza ogni campo, distinguendo `PRESENTE`, `MANCANTE`, `INCOMPLETO`, `NON APPLICABILE / DA VALUTARE`.
3. Indica dove è stato trovato il campo nella bozza o perché manca.
4. Non inventare un campo mancante e non assumere che l’elenco sia completo sul piano giuridico.
5. Ordina per priorità operativa i punti da verificare a cura dell’ufficio.

## Output richiesto
- Intestazione: **BOZZA — Controllo formale preliminare**.
- Tabella `Campo atteso | Esito | Evidenza nella bozza | Azione dell’operatore`.
- Elenco sintetico `Punti da completare`.
- Nota obbligatoria: **Questo confronto riguarda solo lo schema fornito; non certifica conformità normativa né regolarità dell’atto.**

## Regole comuni (contesto PA, uso didattico)
- Lavora **esclusivamente** sui documenti forniti dall’utente per il caso in corso. Non fare ricerche esterne né inventare norme, prassi, referenti, numeri, date, importi, contatti o collegamenti.
- Non accedere a sistemi esterni, non inviare comunicazioni, non registrare o modificare dati. Produci soltanto una **bozza di supporto**.
- Se non trovi un’informazione necessaria, scrivi **NON PRESENTE NELLE FONTI**. Se è ambiguo o richiede valutazione, segnala **DA VERIFICARE**.
- Quando è possibile, indica il punto della fonte a sostegno di ogni informazione rilevante.
- Non trattare dati personali reali in questa esercitazione; gli esempi sono completamente inventati.
- Non dichiarare mai il testo conforme, approvato o pronto per la firma. La verifica spetta alla persona competente.
