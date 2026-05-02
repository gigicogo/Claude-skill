---
name: venezia-elezioni-briefing
description: >
  Genera un briefing giornaliero sulle elezioni comunali di Venezia raccogliendo notizie
  da fonti locali specifiche, con abstract per ogni articolo rilevante e sezione dedicata
  ai candidati. Usa questa skill OGNI VOLTA che l'utente chiede notizie, aggiornamenti,
  rassegna stampa, briefing o sintesi sulle elezioni comunali di Venezia, sul Sindaco di
  Venezia, sui candidati sindaco veneziani, o sulle elezioni a Venezia. Attivala anche
  con frasi come "cosa c'è di nuovo a Venezia", "briefing veneziano", "rassegna stampa
  Venezia elezioni", "aggiornamenti candidati Venezia".
---

# Skill: Venezia Elezioni — Briefing Giornaliero

Questa skill raccoglie, filtra e sintetizza le notizie sulle elezioni comunali di Venezia
da fonti locali autorevoli, producendo un briefing strutturato in markdown con abstract
per ogni articolo rilevante.

---

## FONTI DA MONITORARE

Effettua web_fetch su ciascuno di questi URL (non saltarne nessuno):

1. https://www.ilgazzettino.it
2. https://www.nuovavenezia.it
3. https://corrieredelveneto.corriere.it
4. https://www.veneziatoday.it
5. https://www.lavocedivenezia.it
6. https://primavenezia.it
7. https://antennatre.medianordest.it/category/tg_venezia/
8. https://www.lapiazzaweb.it
9. https://www.elezioni.venezia.it ← aggiornamento frequente, trattare come fonte primaria

Per ogni fonte usa `web_fetch` per recuperare la homepage o la sezione veneziana.
Se una fonte non è raggiungibile, segnalalo esplicitamente nel report con ⚠️.

---

## CANDIDATI NOTI (lista seed — aggiornare dinamicamente)

Elezioni comunali Venezia: **24–25 maggio 2026** (ballottaggio 7–8 giugno 2026)
Otto candidati sindaco, tutti uomini. Sindaco uscente Luigi Brugnaro non ricandidabile.

| Candidato | Schieramento / Lista | Note |
|-----------|---------------------|------|
| **Simone Venturini** | Centrodestra (FdI, Lega, FI, NM + civiche) | 38 anni, assessore uscente turismo/lavoro; appoggio Azione |
| **Andrea Martella** | Centrosinistra "La Stagione Buona" (PD, M5S, AVS, IV + civiche) | Senatore, segretario regionale PD |
| **Claudio Vernier** | "Città vive" (civica indipendente) | Titolare caffè Todaro, radicalismo civico anti-partiti |
| **Michele Boldrin** | "Ora – il coraggio dell'ovvio" | Economista liberal-riformista, già 4,32% alle suppletive venete |
| **Roberto Agirmo** | "Resistere Veneto" | Imprenditore turistico, indipendentista veneto, area free-vax |
| **Luigi Corò** | "Futuro per Venezia Mestre" | Ottavo candidato a sorpresa; vicino a Futuro Nazionale (Vannacci) |
| **Giovanni Andrea Martini** | "Tutta la città che vogliamo" (2 liste civiche) | Ex presidente Municipalità; in rotta con Martella |
| **Pierangelo Del Zotto** | "Prima il Veneto" | Ex assessore provinciale, autonomista, ex Lega |

Se nei testi vengono citati aggiornamenti su questi candidati o nuovi sviluppi,
registrarli nella colonna "Note" con data e breve descrizione.

---

## CRITERI DI FILTRAGGIO

Includi notizie che riguardano:
- Candidature, dichiarazioni, programmi dei candidati sindaco
- Coalizioni, alleanze, accordi tra partiti per le elezioni comunali
- Sondaggi e proiezioni elettorali
- Temi cittadini con impatto elettorale esplicito o implicito:
  - Grandi navi / crocieristica
  - Overtourism e residenzialità
  - Porto di Venezia
  - Mose e gestione lagunare
  - Trasporti locali (ACTV, parcheggi)
  - Emergenza abitativa
  - Qualsiasi tema su cui i candidati si differenziano o prendono posizione

Escludi notizie senza alcuna rilevanza elettorale (cronaca nera generica, sport, meteo, ecc.)
a meno che non abbiano un aggancio diretto con la campagna elettorale.

---

## STRUTTURA DEL BRIEFING

Genera il documento seguendo ESATTAMENTE questo schema markdown:

```
# 🗳️ Briefing Elezioni Comunali Venezia
**Data:** [DATA ODIERNA]
**Fonti monitorate:** [N]/8 raggiunte

---

## 📌 Sintesi del giorno
[3-5 righe che riassumono i temi più rilevanti emersi oggi, con tono analitico]

---

## 👤 Candidati in campo

| Candidato | Coalizione/Partito | Ultimo aggiornamento |
|-----------|-------------------|----------------------|
| [Nome]    | [Partito/i]       | [breve nota]         |

---

## 📰 Notizie per fonte

### [Nome Fonte]
#### [Titolo articolo]
**Fonte:** [URL articolo se disponibile]
[Abstract di 3 righe: cosa è successo, chi è coinvolto, rilevanza elettorale]

---

## 🔍 Temi caldi oggi
Elenco puntato dei macro-temi emersi oggi con il numero di fonti che ne parlano.

---

## ⚠️ Note operative
[Fonti non raggiungibili, errori di fetch, anomalie]
```

---

## ISTRUZIONI DI ESECUZIONE

1. **Fetch delle fonti**: recupera tutte le 8 fonti con `web_search` o `web_fetch`.
   Prioritizza `web_fetch` per le homepage. Se `web_fetch` fallisce, usa `web_search`
   con query: `site:[dominio] elezioni venezia sindaco 2025` come fallback.

2. **Filtraggio**: applica i criteri di filtraggio. Scarta notizie irrilevanti.

3. **Abstract**: per ogni notizia rilevante, scrivi UN titolo + 3 righe di abstract.
   Le 3 righe devono rispondere a: (1) cosa è successo, (2) chi è coinvolto,
   (3) perché conta per le elezioni.

4. **Candidati**: identifica i candidati citati, aggiorna la tabella.
   Se un candidato è citato per la prima volta, aggiungi "(nuovo)" nella colonna note.

5. **Output doppio**:
   - Mostra il markdown completo in chat (renderizzato)
   - Salva il file come `briefing-venezia-YYYY-MM-DD.md` in `/mnt/user-data/outputs/`
     e presentalo con `present_files` per il download

6. **Tono**: analitico, neutro, non di parte. Se un articolo è palesemente di
   orientamento politico, segnalarlo nell'abstract con una nota breve.

---

## GESTIONE ERRORI

- Se una fonte restituisce errore o è irraggiungibile: segnala con ⚠️ e prosegui
- Se nessuna fonte ha notizie elettorali oggi: produrre il briefing vuoto con nota esplicita
- Non inventare notizie. Se non c'è nulla, scrivilo.
- Se il contenuto di una pagina è ambiguo o non parsabile, usa web_search come fallback
