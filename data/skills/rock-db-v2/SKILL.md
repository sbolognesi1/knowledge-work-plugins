---
name: rock-db-v2 schema and workflow
description: Domain knowledge for querying and extending rock-db-v2, a SQLite album ranking aggregator combining Rolling Stone, NME, Pitchfork, Metal Hammer, and scaruffi.com scores with MusicBrainz enrichment.
---

# rock-db-v2 — Album Ranking Aggregator

## Cos'è
Database SQLite che aggrega classifiche album da più fonti critiche (Rolling Stone, NME, Pitchfork, Metal Hammer, scaruffi.com) in un punteggio composito, arricchito con metadati MusicBrainz.

## Stato dati
- Scraper scaruffi.com ha importato ~4750 righe
- Enrichment MusicBrainz completo
- Lavoro in corso: `propose_scaruffi_title_fixes.py` per 31 titoli con parentesi label/score residue

## Come interrogare
Stack: Python 3.13, SQLite, pandas. Query dirette via `sqlite3` CLI o pandas `read_sql`.

## Metodologia di riferimento
Composite scoring ispirato a Dave Fernig (2015).

## Quando usare questa skill
Attivala per: query sul database, analisi punteggi compositi, debug enrichment MusicBrainz, pulizia titoli scaruffi.
