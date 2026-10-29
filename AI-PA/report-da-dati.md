---
name: report-da-dati
description: "Usa questa skill quando l’utente fornisce una tabella già verificata e richiede una sintesi descrittiva e numerica, senza attribuire cause ai fenomeni non dimostrate dai dati."
---

# Report da dati

## Scopo
Trasformare una piccola tabella fornita dall’utente in un commento descrittivo accurato, separando numeri, calcoli e interpretazioni.

## Input da richiedere
- Tabella CSV o dati tabellari, con definizione delle colonne e unità di misura.
- Periodo di riferimento e destinatario del report.

## Procedura
1. Leggi esattamente colonne, periodi, valori e unità; se mancano definizioni chiedi chiarimenti.
2. Esegui soltanto calcoli riproducibili: somme, differenze, quote e percentuali, specificando denominatori.
3. Riporta i dati senza confondere richieste ricevute con richieste evase o confermate.
4. Evita inferenze causali, previsioni, giudizi sulle prestazioni o confronti esterni se non documentati.
5. Indica eventuali anomalie, campi mancanti o limiti della tabella.
6. Se possibile, mostra esplicitamente almeno un esempio di formula usata nei calcoli.

## Output richiesto
- Titolo: **BOZZA — Report descrittivo da verificare**.
- `Tre dati essenziali`.
- `Andamento del periodo` (max 140 parole).
- Tabella `Indicatore | Calcolo | Risultato`.
- `Limiti dei dati e verifiche necessarie`.
- Avvertenza: **L’analisi non costituisce una valutazione o decisione amministrativa.**

## Regole comuni (contesto PA, uso didattico)
- Lavora **esclusivamente** sui documenti forniti dall’utente per il caso in corso. Non fare ricerche esterne né inventare norme, prassi, referenti, numeri, date, importi, contatti o collegamenti.
- Non accedere a sistemi esterni, non inviare comunicazioni, non registrare o modificare dati. Produci soltanto una **bozza di supporto**.
- Se non trovi un’informazione necessaria, scrivi **NON PRESENTE NELLE FONTI**. Se è ambiguo o richiede valutazione, segnala **DA VERIFICARE**.
- Quando è possibile, indica il punto della fonte a sostegno di ogni informazione rilevante.
- Non trattare dati personali reali in questa esercitazione; gli esempi sono completamente inventati.
- Non dichiarare mai il testo conforme, approvato o pronto per la firma. La verifica spetta alla persona competente.
