# Vejledning: Setup og Brug af Git i VS Code

Dette dokument er en praktisk vejledning til, hvordan du bruger **VS Code (Visual Studio Code)** til at redigere dine jobansøgninger og synkronisere dem med din hjemmeside på GitHub via Git.

---

## 1. Grundlæggende opsætning (Engangsopsætning)

For at sikre, at Git og VS Code arbejder perfekt sammen, kan du konfigurere VS Code som standard-tekstredigeringsprogram for Git.

### Sæt VS Code som standard Git-editor
Åbn en terminal og kør følgende kommando:
```bash
git config --global core.editor "code --wait"
```
*Dette gør, at hvis Git har brug for, at du skriver en besked (f.eks. ved et merge), åbner den automatisk i et VS Code-vindue.*

---

## 2. Daglig arbejdsgang i VS Code (GUI / Visuel menu)

Dette er den nemmeste og mest anbefalede metode. Du behøver ikke skrive kommandoer i terminalen.

### Trin 1: Åbn dit projekt
1. Åbn **VS Code**.
2. Vælg **File** -> **Open Folder...** (Åbn mappe).
3. Vælg mappen: `/var/home/haj/Documents/job/ansøgninger`.

### Trin 2: Lav dine ændringer
1. Klik på den fil, du vil redigere (f.eks. `index.html` eller `cv/index.html`).
2. Foretag dine ændringer i teksten.
3. Gem filen ved at trykke på `Ctrl + S`.

### Trin 3: Klargør ændringer (Stage)
1. Klik på **Source Control**-ikonet i venstre sidebjælke (tre cirkler forbundet med streger - genvej: `Ctrl + Shift + G`).
2. Du vil se dine ændrede filer under listen **Changes**.
3. Hold musen over den fil, du vil gemme, og klik på **`+`-ikonet** ("Stage Changes"). Filen flytter sig nu op under **Staged Changes**.

### Trin 4: Gem ændringerne lokalt (Commit)
1. I tekstfeltet øverst (hvor der står *Message*), skriver du en kort besked om, hvad du har rettet (f.eks. `Opdateret telefonnummer` eller `Rettet stavefejl i CV`).
2. Klik på den blå **Commit**-knap. Ændringerne er nu gemt i din lokale historik på computeren.

### Trin 5: Send ændringerne til GitHub (Sync / Push)
1. Klik på den blå knap **Sync Changes** (eller klik på de tre prikker `...` øverst i Git-panelet og vælg **Push**).
2. Inden for ca. 1 minut vil din hjemmeside være opdateret live på internettet!

---

## 3. Alternativ arbejdsgang: Terminal (Kommandoer)

Hvis du foretrækker at bruge terminalen i bunden af VS Code (genvej: `Ctrl + \``):

1. **Se hvilke filer der er ændret:**
   ```bash
   git status
   ```
2. **Klargør filen (Stage):**
   ```bash
   git add referat_github_pages.md
   ```
   *(Brug `git add .` for at klargøre alle ændrede filer på én gang).*
3. **Gem lokalt (Commit):**
   ```bash
   git commit -m "Beskriv din ændring her"
   ```
4. **Send til GitHub Pages (Push):**
   ```bash
   git push origin main
   ```

---

## 4. Oversigt over dine lokale filer og links

Her er genveje til dine vigtigste filer i mappen, som du kan åbne direkte i VS Code:

* **IT-Ansøgning (HOFOR):** [index.html](file:///var/home/haj/Documents/job/ansøgninger/index.html)
* **IT-CV:** [cv/index.html](file:///var/home/haj/Documents/job/ansøgninger/cv/index.html)
* **Pædagog-CV:** [paedagog/cv/index.html](file:///var/home/haj/Documents/job/ansøgninger/paedagog/cv/index.html)
* **Molevitten ansøgning:** [paedagog/molevitten/index.html](file:///var/home/haj/Documents/job/ansøgninger/paedagog/molevitten/index.html)
* **Sjællandsbroen ansøgning:** [paedagog/sjaellandsbroen/index.html](file:///var/home/haj/Documents/job/ansøgninger/paedagog/sjaellandsbroen/index.html)
* **GitHub Pages Referat:** [referat_github_pages.md](file:///var/home/haj/Documents/job/ansøgninger/referat_github_pages.md)
