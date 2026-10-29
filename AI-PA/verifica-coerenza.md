---
name: verifica-coerenza
description: "Usa questa skill quando l’utente fornisce un documento di riferimento e un testo derivato (sintesi, FAQ, bozza o comunicazione) e vuole identificare affermazioni contrastanti, omissioni o alterazioni rispetto alla fonte."
---

# Verifica di coerenza

## Scopo
Cercare possibili incoerenze tra una fonte e un testo derivato, senza riscrivere automaticamente la bozza.

## Input da richiedere
- Documento **fonte** (identificato come FONTE).
- Documento da controllare (identificato come BOZZA).

## Procedura
1. Leggi **prima** la fonte e individua fatti, condizioni, scadenze, eccezioni e limiti.
2. Esamina la bozza frase per frase e trova affermazioni riscontrabili nella fonte.
3. Segnala: `CONTRADDIZIONE`, `INFORMAZIONE NON SUPPORTATA`, `OMISSIONE RILEVANTE`, `DA VERIFICARE`.
4. Per ciascuna segnalazione, cita brevemente il passaggio della **fonte** e il passaggio della **bozza**.
5. Se non rilevi problemi, scrivi `NESSUN PROBLEMA INDIVIDUATO IN QUESTA ANALISI`, senza attestare la correttezza.
6. Non correggere, completare o pubblicare il documento: lascia la decisione di modificare alla persona competente.

## Output richiesto
- Intestazione: **BOZZA — Segnalazioni di coerenza da verificare**.
- Tabella `N. | Passaggio della bozza | Tipo di problema | Cosa dice la fonte | Punto della fonte | Priorità`.
- Nota finale: `La persona competente deve verificare direttamente i testi originali`.

## Regole comuni (contesto PA, uso didattico)
- Lavora **esclusivamente** sui documenti forniti dall’utente per il caso in corso. Non fare ricerche esterne né inventare norme, prassi, referenti, numeri, date, importi, contatti o collegamenti.
- Non accedere a sistemi esterni, non inviare comunicazioni, non registrare o modificare dati. Produci soltanto una **bozza di supporto**.
- Se non trovi un’informazione necessaria, scrivi **NON PRESENTE NELLE FONTI**. Se è ambiguo o richiede valutazione, segnala **DA VERIFICARE**.
- Quando è possibile, indica il punto della fonte a sostegno di ogni informazione rilevante.
- Non trattare dati personali reali in questa esercitazione; gli esempi sono completamente inventati.
- Non dichiarare mai il testo conforme, approvato o pronto per la firma. La verifica spetta alla persona competente.
