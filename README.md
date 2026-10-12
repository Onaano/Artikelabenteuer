# 🧭 Artikel-Abenteuer — Der, die, das • ein & eine

Interaktives Deutsch-Lernspiel für **Klasse 1–2, Schuleingangsphase, Förderunterricht, Sprachförderung und DaZ**.
Nomen werden **zusammen mit ihrem Artikel** als Einheit gelernt (DER BALL, DIE BLUME, DAS BUCH, EIN BALL, EINE BLUME, EIN BUCH).
Nur **Nominativ Singular** – keine Akkusativ-, Dativ- oder Genitivformen.

## 🎮 Die sechs Modi (Abenteuerorte)
1. **Der, die oder das?** (Weggabelung) – Bild + Wort hören, Artikel wählen; danach groß „DER BALL“ und Sprachausgabe „der Ball“.
2. **Pack den Rucksack!** (Entdeckercamp) – 3 / 4–5 / 5–6 Bildkarten in die Rucksäcke DER / DIE / DAS sortieren (Ziehen mit Maus/Finger **oder** Antippen). Danach alle Kombinationen sichtbar und nacheinander gesprochen.
3. **Was gehört zusammen?** (Alte Brücke) – Wörter und Artikel paarweise verbinden (Leicht: nur Bilder, Mittel: Bild + Wort, Schwer: Wörter; ab Mittel teils EIN/EINE).
4. **Welcher Artikel fehlt?** (Höhle, ab Mittel) – Nominativ-Sätze mit Lücke („___ Hund schläft.“, „Hier steht ___ Lampe.“). Die Aufgabe nennt immer, ob der/die/das oder ein/eine gesucht ist.
5. **Ein oder eine?** (Schatzkammer) – Verbindung DER BALL ↓ EIN BALL sichtbar; Sprachausgabe „ein Ball“.
6. **Gemischt** (Große Schatzsuche) – Rundenplan aus den passenden Modi; nie dieselbe Aufgabenart direkt hintereinander. Leicht: vor allem der/die/das mit Bild und Ton.

**Eine Runde = 8 richtig gelöste Aufgaben** (nicht Versuche). Auf der Abenteuerkarte läuft der Entdecker pro Aufgabe eine Station weiter bis zur Schatztruhe. Danach „Abenteuer geschafft!“ mit „Noch eine Runde“ / „Zurück zur Auswahl“.
Kein Zeitlimit, keine Punkte, keine Leben, kein Game Over, keine Highscores. Falsche Antwort = freundlicher Hinweis („Hör dir das Wort noch einmal an.“), die Aufgabe bleibt, es gibt keinen Fortschritt, **die Lösung wird nicht verraten**.

## 🔤 Wortschatz
**96 kuratierte Nomen** (der 36 · die 33 · das 27), Standardsprache, eindeutiges Genus, keine Eigennamen, keine Abstrakta in „Leicht“. Jeder Eintrag hat:
`word, definiteArticle, indefiniteArticle, gender, difficulty, category, illustration` (+ Bildgruppe für ähnlich aussehende Bilder).
Bild, Wort, Artikel und Sprachausgabe kommen **immer aus demselben Datensatz**. ein/eine: der → ein, die → eine, das → ein.
Stufen: Leicht = 40 häufige Alltagswörter · Mittel = leicht + mittel · Schwer = mittel + schwer (Wörter wie Kompass, Fernglas, Schatztruhe).
Mehrdeutige Wörter wurden bewusst ausgelassen (z. B. „der/die Leiter“, „der/das Schloss“, „der/das See“). Alle Artikel wurden unabhängig gegen Wiktionary-Daten (Python-Paket *german-nouns*) geprüft.
Prüfübersicht mit Bildern: `pruefung/wortliste.html`, `.pdf`, `.csv`.

## 🔀 Abwechslung & Eindeutigkeit
- Rundenplan zu Rundenbeginn: kein Nomen doppelt pro Runde, Artikel ausgewogen, gemischte Kategorien, ähnlich aussehende Bilder (z. B. Katze/Tiger/Löwe) nie gemeinsam.
- **Farben und Positionen sind nie an einen Artikel gebunden:** Knopf-/Rucksackfarben werden pro Aufgabe zufällig aus fünf neutralen Varianten vergeben, die richtige Antwort steht gleichmäßig links/Mitte/rechts.
- **Rucksack:** Die Reihenfolge der Karten wird so gewählt, dass der richtige Rucksack fast nie direkt unter der Karte liegt (geprüft: nur ca. 11 % der Karten statt 33 % bei reinem Zufall) – Kinder können sich also keine Position merken, sondern müssen den Artikel wissen.
- Lücken-Sätze: nur Nominativ-Vorlagen („___ N schläft.“, „Hier steht/liegt/ist ___ N.“, „___ N ist da.“), je Aufgabe passt genau **ein** Artikel.

## 🔊 Sprachausgabe
Browser-Sprachausgabe (de-DE). Vor der Aufgabe wird nur das Nomen gesprochen, nach der Lösung immer die vollständige Wendung („der Ball“, „ein Ball“). Das Wort steht **immer** sichtbar da (auch in „Leicht“, auch wenn es gehört wird) – so lässt sich das Spiel auch ohne Ton spielen.

## 📱 Geräte & Bedienung
Smartboard, PC, Laptop, Tablet, Smartphone; Maus, Touch, Tastatur; Hoch- und Querformat (Querformat: Bild links, Bedienung rechts). Alle Aufgaben passen **ohne Scrollen** (geprüft von 360×640 bis 2560×1440, Laptop ab ca. 600 px Höhe). Touch-Ziele ≥ 44 px, sichtbare Fokusrahmen, Kontraste nach WCAG AA, `prefers-reduced-motion`.

## 🛠️ Technik
Eine einzige `index.html` (HTML, CSS, Vanilla JavaScript). Keine Frameworks, keine externen Bilder/Schriften/APIs, keine Cookies, kein Tracking, keine Datenspeicherung.
Netlify: Ordner per Drag & Drop (Build command leer, Publish directory `.`). GitHub: `index.html`, `README.md`, `.gitignore` (+ optional `arbeitsblaetter/`, `pruefung/`).

## 🖨️ Arbeitsmaterialien (`arbeitsblaetter/`, HTML + PDF)
- `teilnehmeruebersicht` – A4 quer, 30 Kinder × 10 Runden
- `arbeitsblatt-der-die-das` – Bilder zuordnen, Artikel ergänzen, Wörter sortieren, Artikel mit Wort verbinden
- `arbeitsblatt-ein-eine` – EIN/EINE ergänzen, DER BALL → EIN BALL verbinden, Bildwörter schreiben, Bilder zuordnen
- jeweils zusätzlich `-loesung` (für Lehrkräfte). Bilder und Lösungen wurden aus dem fertigen HTML nachgeprüft.

## ✅ Qualitätssicherung
Daten-/Grammatik-Audit über 42.500 simulierte Runden (Artikel, ein/eine-Zuordnung, genau eine Lösung je Aufgabe, nur Nominativ-Sätze, Verteilung, keine Wortwiederholung, Stufen) · alle 6 Modi × 3 Stufen als volle Runden über die Oberfläche (Fortschritt, Sprachphrasen, Ende, „Noch eine Runde“) · falsche Antworten ohne Fortschritt · Drag & Drop mit Maus und Touch + Tippen-Alternative · Tastatur · Betrieb ohne Sprachausgabe · Reduced Motion · Kontrastprüfung · 16 Bildschirmgrößen ohne Scrollen/Überlappung/horizontalen Balken · Konsole ohne Fehler.
