# InvestorHub

5 Tools für smarte Privatinvestoren.

## Tools

1. **Stress Lab** – Portfolio-Crashtest gegen 5 historische Krisen
2. **Dividend Snowball** – Zinseszins-Effekt von Dividenden visualisieren
3. **Opportunity Cost** – Wahre Kosten deines Lifestyles + Joy-Value-Schwelle
4. **Rebalancing Radar** – Drift erkennen, konkrete Handlungsanweisungen in EUR
5. **FIRE Dashboard** – Freedom Date, Monte-Carlo-Simulation, Coast-FIRE

## Setup

1. Repository klonen oder forken
2. GitHub Settings → Pages → Source: "main" → Save
3. App öffnen → Anthropic API-Key eingeben (einmalig, wird lokal gespeichert)
4. Wertpapiere per WKN/ISIN suchen oder manuell eingeben

## Sicherheit

- API-Key wird nur im localStorage deines Browsers gespeichert, nicht im Code
- Alle Inputs werden sanitized (HTML, Control-Chars, Injection-Patterns)
- API-Responses werden strukturell validiert bevor sie gerendert werden
- Empfehlung: Spending-Limit in der Anthropic Console setzen (z.B. 5€/Monat)
- Keine externen Abhängigkeiten außer React (unpkg CDN) und Google Fonts

## Technik

- Single-File HTML – kein Build-Step nötig
- React 18 via CDN
- localStorage für Portfolio und API-Key
- Responsive: optimiert für Desktop bis 250px Breite
- PWA-fähig (Add to Home Screen auf iOS/Android)
