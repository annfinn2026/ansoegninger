# Vejledning & Referat: GitHub Pages for Jobansøgninger

Dette dokument opsummerer det arbejde, vi har udført for at flytte din jobmappe væk fra `duckdns.org` og over på en langt mere professionel og stabil platform: **GitHub Pages**.

---
**Resume: agy --conversation=bb983996-0a2c-4124-8a19-9c9f25547f40 (or -c)**
**Resume: agy --conversation=b51029b4-a435-40ad-a815-a0c6f27dd85e (or -c)**

## 1. Hvad vi har ændret og hvorfor
* **Platformskift:** Vi er flyttet fra `myndir.duckdns.org` til **GitHub Pages**. Dynamic DNS (som DuckDNS) bliver ofte blokeret af virksomheders firewalls og kan se mistænkeligt ud. GitHub Pages har maksimal troværdighed hos IT-systemer og arbejdsgivere.
* **Format:** Dine ansøgninger, CV og pædagogbevis er nu alle tilgængelige som interaktive, designbeskyttede **HTML-sider** i stedet for PDF-filer.
* **Rene links (Clean URLs):** Vi har fjernet filendelserne (`.html`) og grimme tegn (som `ø` og mellemrum) fra internetadresser ved at oprette en standardiseret mappestruktur.

---

## 2. Din nye filstruktur (lokalt)
I din lokale mappe `/var/home/haj/Documents/job/ansøgninger/` har vi oprettet følgende struktur:

### IT-supporter
* `index.html` *(Ansøgning til IT-supporter hos HOFOR)*
* `cv/index.html` *(Dit IT-CV)*

### Pædagog
* `paedagog/cv/index.html` *(Dit pædagog-CV - førhen `cv_design.html`)*
* `paedagog/molevitten/index.html` *(Ansøgning til Molevitten - førhen `molevitten.html`)*
* `paedagog/falkonergaarden/index.html` *(Ansøgning til Falkonergården - førhen `falkonergaarden.html`)*
* `paedagog/sjaellandsbroen/index.html` *(Ansøgning til Sjællandsbroen - førhen `sjaellandsbroen.html`)*

### Fælles bilag
* `bevis/index.html` *(Dit pædagogiske uddannelsesbevis)*

---

## 3. Dine nye links på internettet
Efter du har aktiveret GitHub Pages, er dine dokumenter tilgængelige på følgende adresser:

### IT-Job Links
* **Hovedansøgning (HOFOR):**  
  [https://annfinn2026.github.io/ansoegninger/](https://annfinn2026.github.io/ansoegninger/)
* **Dit IT-CV:**  
  [https://annfinn2026.github.io/ansoegninger/cv/](https://annfinn2026.github.io/ansoegninger/cv/)

### Pædagog-Job Links
* **Dit Pædagog-CV:**  
  [https://annfinn2026.github.io/ansoegninger/paedagog/cv/](https://annfinn2026.github.io/ansoegninger/paedagog/cv/)
* **Ansøgning (Molevitten):**  
  [https://annfinn2026.github.io/ansoegninger/paedagog/molevitten/](https://annfinn2026.github.io/ansoegninger/paedagog/molevitten/)
* **Ansøgning (Falkonergården):**  
  [https://annfinn2026.github.io/ansoegninger/paedagog/falkonergaarden/](https://annfinn2026.github.io/ansoegninger/paedagog/falkonergaarden/)
* **Ansøgning (Sjællandsbroen):**  
  [https://annfinn2026.github.io/ansoegninger/paedagog/sjaellandsbroen/](https://annfinn2026.github.io/ansoegninger/paedagog/sjaellandsbroen/)

### Uddannelsesbevis
* **Uddannelsesbevis:**  
  [https://annfinn2026.github.io/ansoegninger/bevis/](https://annfinn2026.github.io/ansoegninger/bevis/)

*Bemærk: Alle links internt er blevet opdateret, så Pædagog-siderne linker til dit Pædagog-CV, og IT-siderne linker til dit IT-CV.*

---

## 4. Fremtidig arbejdsgang (Workflow)

Du har nu fuld integration mellem din computer og din live-hjemmeside. Her er, hvordan du opdaterer dine filer fremover.

### Metode A: Gennem VS Code (Anbefalet)
Dette er den hurtigste og mest professionelle måde at arbejde på:

1. Åbn mappen `ansøgninger` i **VS Code**.
2. Lav dine ændringer i koden (f.eks. justering af tekst i `index.html` eller `cv/index.html`) og gem (`Ctrl + S`).
3. Klik på **Source Control**-ikonet i VS Codes venstre side (tre cirkler forbundet af streger).
4. Skriv en kort besked i beskedfeltet (f.eks. `Rettet telefonnummer` eller `Opdateret CV`).
5. Klik på den blå knap **Commit**.
6. Klik på **Sync Changes** (eller *Push*) for at sende ændringerne op.
7. *Efter ca. 1 minut er hjemmesiden opdateret på internettet!*

### Metode B: Direkte i browseren på GitHub.com
Til små hurtige rettelser (f.eks. en stavefejl), hvis du ikke sidder ved din egen computer:

1. Gå til [github.com/annfinn2026/ansoegninger](https://github.com/annfinn2026/ansoegninger).
2. Klik på den fil, du vil ændre (f.eks. `index.html`).
3. Klik på **blyant-ikonet** ("Edit this file") øverst til højre.
4. Ret teksten.
5. Klik på **Commit changes...** i øverste højre hjørne for at gemme og udgive.
