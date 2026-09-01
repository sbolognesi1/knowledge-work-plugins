---
name: scaruffi-project schema and workflow
description: Domain knowledge for scaruffi-project, a Flask + D3.js interactive visualization of Scaruffi's music database with PageRank-based node importance.
---

# scaruffi-project — Visualizzazione Interattiva Database Scaruffi

## Cos'è
Applicazione Flask + D3.js v7 per esplorare visivamente il database musicale di scaruffi.com come grafo interattivo.

## Architettura
- Backend: Flask
- Frontend: D3.js v7
- Scraper con exponential backoff
- PageRank (via networkx) calcolato una sola volta in fase di scraping, salvato in `nodes.csv`

## Design
Estetica "Minimal Brutalism": off-white `#F5F2EC`, nero `#0A0A0A`, rosso `#E01A1A`, font Space Grotesk peso 900.

## Come interrogare
Stack: Python, Flask, networkx, pandas, D3.js. Dati statici pre-calcolati in `nodes.csv` (non ricalcolare PageRank ad ogni richiesta).

## Quando usare questa skill
Attivala per: debug scraping, modifiche al grafo/visualizzazione D3, questioni di layout/design Brutalist, calcoli PageRank.
