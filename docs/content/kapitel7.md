# Kapitel 7 – Prompt-Hacks für den Marketing-Alltag

{{ progress(7) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Wie der **Rückfragen-Prompt** und der **Flipped-Prompt** die Arbeitsrichtung umdrehen
- Wie du mit dem **Varianten-Fächer** und der **Selbstkritik-Schleife** schneller zu besseren Texten kommst
- Wie du per **Stil-Extraktion** aus Beispieltexten eine wiederverwendbare Beschreibung der **Markenstimme** gewinnst
- Wie **Perspektivwechsel** und präzise **Umschreibe-Befehle** Texte gezielt verbessern
- Wie du **benutzerdefinierte Anweisungen**, **Projekte** und **Memory** sinnvoll und datensparsam einsetzt
- Welche verbreiteten „Hacks" **Mythen** sind – und warum sie trotzdem weitergegeben werden
</div>

---

## 7.1 Rückfragen-Prompt und Flipped-Prompt

Kapitel 5 und 6 haben gezeigt, wie du einen Auftrag vollständig formulierst. Im Alltag fehlt dir dafür manchmal die Zeit – oder du weißt selbst noch nicht genau, was du brauchst. Zwei Hacks drehen dann die Arbeitsrichtung um: Nicht du lieferst alles, sondern das Werkzeug fragt nach.

**Der Rückfragen-Prompt** hängt an einen knappen Auftrag eine Bitte um Rückfragen an:

```text
Ich brauche einen Newsletter zum Saisonstart im Frühjahr für Fjordlicht.
Bevor du schreibst: Stelle mir die fünf wichtigsten Fragen, deren
Antworten den Text am stärksten verbessern. Nummeriere sie und warte
auf meine Antworten.
```

Die Rückfragen zeigen dir, welche Bausteine fehlen – meist Purpose, Fakten und Länge. Beantworte sie kurz, und notiere sie dir: Was hier gefragt wird, gehört beim nächsten Mal direkt in deinen Prompt-Canvas (Kap. 5).

**Der Flipped-Prompt** (Umkehr-Prompt) geht einen Schritt weiter: Das Werkzeug interviewt dich und schreibt am Ende den Prompt, den du dann verwendest.

```text
Du hilfst mir, einen guten Prompt für folgende Aufgabe zu schreiben:
[Aufgabe in einem Satz].
Interviewe mich dazu. Stelle immer nur eine Frage auf einmal und warte
auf meine Antwort. Wenn du genug weißt, schreibe den fertigen Prompt
nach dem P.R.O.M.P.T.-Schema: Persona, Request, Output, Modifier,
Purpose, Tone.
```

| Hack | Wann nutzen | Vorteil | Grenze |
|---|---|---|---|
| **Rückfragen-Prompt** | Auftrag ist klar, Details fehlen | schnell, deckt Lücken auf | Fragen sind manchmal allgemein |
| **Flipped-Prompt** | neue Aufgabe, eigenes Bild noch unscharf | strukturiert dein Denken | dauert länger, Ergebnis kann überladen sein |

!!! tip "Ein Satz für die Zwischenablage"
    „Stelle mir zuerst Fragen" ist der Hack mit dem besten Verhältnis von Aufwand zu Wirkung. Lege den Satz als Textbaustein ab, zum Beispiel in der Tastaturkürzel-Funktion deines Betriebssystems, und hänge ihn an jeden Auftrag an, bei dem du unsicher bist.

---

## 7.2 Varianten-Fächer und Selbstkritik-Schleife

Ein einzelner Entwurf verleitet dazu, ihn zu übernehmen, weil er „ganz okay" ist. Der **Varianten-Fächer** zwingt dich zur Auswahl – und zwingt das Modell, unterschiedliche Richtungen auszuprobieren statt Synonyme.

```text
Schreibe fünf Betreffzeilen für den Newsletter zum Rucksack Tind.
Jede Variante folgt einem anderen Ansatz:
1. Nutzen, 2. Neugier, 3. Situation aus dem Alltag, 4. Frage,
5. trockener Humor.
Gib zu jeder Variante in einem Halbsatz an, für welche Leser sie
am besten passt.
```

Der Trick liegt in der Vorgabe **unterschiedlicher Ansätze**. Ohne sie bekommst du fünf Varianten desselben Satzes. Aus dem Fächer wählst du zwei aus, die du im Newsletter-Tool gegeneinander testest (Kap. 16).

Die **Selbstkritik-Schleife** lässt das Modell den eigenen Entwurf gegen Kriterien prüfen und überarbeiten:

```text
Prüfe deinen Entwurf gegen diese Kriterien und gib zu jedem
Kriterium eine Note von 1 bis 5 mit einem Satz Begründung:
- Konkreter Nutzen für die Leserin im ersten Satz
- Markenstimme: ruhig, ehrlich, keine Superlative
- Nur Fakten aus dem Produktblatt
- Klare Handlungsaufforderung am Ende
Überarbeite danach alle Punkte unter 4 und gib die neue Fassung aus.
```

!!! warning "Typische Falle"
    Die Selbstkritik läuft im selben System, das den Text geschrieben hat. Sie findet **formale** Schwächen zuverlässig – Länge, fehlende Handlungsaufforderung, Superlative. Sie findet **nicht** zuverlässig eine erfundene Zahl, denn das Modell hält sie für richtig. Ohne konkrete Kriterien („Prüfe deine Antwort") ist die Schleife fast wirkungslos. Schärfer wird es mit dem Rollenwechsel im neuen Chat (Kap. 6).

---

## 7.3 Stil-Extraktion: die Markenstimme aus Beispielen gewinnen

Viele Unternehmen haben keinen Styleguide – oder einen, der nur „modern, sympathisch, kompetent" sagt. Gleichzeitig gibt es Texte, die alle für gelungen halten. Die **Stil-Extraktion** macht aus diesen Texten eine präzise Beschreibung, die du in jeden Prompt einsetzen kannst.

```text
Analysiere die drei Texte in <beispiele>. Sie zeigen unsere Markenstimme.
Beschreibe den Stil so, dass eine andere Person damit neue Texte im
gleichen Ton schreiben kann. Gliedere in:
1. Tonalität in Gegensatzpaaren (z. B. ehrlich statt euphorisch)
2. Satzbau und Satzlänge
3. Wortwahl: typische Wörter und Wörter, die nie vorkommen
4. Ansprache und Perspektive
5. Umgang mit Produktvorteilen und Nachhaltigkeit
Nenne zu jedem Punkt ein kurzes Zitat aus den Beispielen als Beleg.
<beispiele>
[drei bis fünf gelungene Texte, gern aus verschiedenen Kanälen]
</beispiele>
```

Das Ergebnis ist ein Entwurf, kein fertiger Styleguide. Prüfe jeden Punkt: Stimmt das wirklich, oder hat das Modell etwas hineingelesen? Dann kürze auf eine halbe Seite. Diese **Brand-Voice-Beschreibung** wird zum festen Tone-Baustein in deinen Prompts und später zum Kern eines Assistenten wie des Content-Assistenten von Fjordlicht (Kap. 26).

| Ergebnis der Extraktion | Gut, wenn … | Nachschärfen, wenn … |
|---|---|---|
| Gegensatzpaare | jedes Paar sich am Text belegen lässt | Paare austauschbar sind („modern statt altmodisch") |
| Wortlisten | konkrete Wörter genannt werden | nur Wortarten oder Allgemeinplätze stehen |
| Satzbau | Länge und Rhythmus beschrieben sind | „abwechslungsreich" die einzige Angabe ist |
| Belege | Zitate tatsächlich aus den Beispielen stammen | Zitate nicht wörtlich auffindbar sind |

!!! info "Merksatz"
    Wer die Markenstimme nur mit Adjektiven beschreibt, bekommt Durchschnitt. Wer sie aus **echten Texten** ableitet und mit Gegensatzpaaren, Wortlisten und Belegen festhält, bekommt Wiedererkennbarkeit.

---

## 7.4 Perspektivwechsel und Umschreibe-Befehle

Beim **Perspektivwechsel** lässt du die Zielgruppe den Text kommentieren. Das ersetzt keine echte Kundenbefragung, deckt aber blinde Flecken auf.

```text
Du bist Mareike, 34, lebst in Münster, fährst mit dem Rad zur Arbeit
und gehst am Wochenende mit deinen zwei Kindern wandern. Du kaufst
lieber weniger, dafür Langlebiges. Lies den folgenden Newsletter und
kommentiere ehrlich: Wo steigst du aus? Was glaubst du nicht?
Was fehlt dir, um zu klicken?
[Newsletter einfügen]
```

Die Antworten sind simuliert – das Modell weiß nicht, was echte Kundinnen denken, sondern was in seinen Trainingsdaten typisch klingt. Nutze den Perspektivwechsel als Anstoß für eigene Überlegungen, nicht als Marktforschung. Wie du solche Figuren als belastbaren Kundenavatar aufbaust, zeigt Kapitel 18.

Für die Überarbeitung bewährt sich ein Repertoire präziser **Umschreibe-Befehle**. Je genauer der Befehl, desto weniger verändert das Modell, was schon gut war.

| Befehl | Wirkung |
|---|---|
| „Kürze auf 60 Wörter, behalte den ersten und den letzten Satz." | kürzt gezielt, Einstieg und Abschluss bleiben |
| „Streiche alle Adjektive, die nichts Überprüfbares sagen." | entfernt Floskeln wie „hochwertig", „innovativ" |
| „Schreibe für Lesestufe einfach: kurze Sätze, keine Fachwörter." | verständlichere Fassung, etwa für Social Media |
| „Ändere nur den Einstieg, alles andere bleibt wörtlich." | schützt den Rest vor ungewollten Änderungen |
| „Formuliere aktiv statt passiv." | lebendiger, klarer Handelnder |
| „Mache aus dem Text drei Stichpunkte für eine Instagram-Story." | Formatwechsel bei gleichem Inhalt |

!!! tip "Gezielt statt global"
    „Mach es besser" führt zu einer komplett neuen Fassung, in der Gelungenes verloren geht. Benenne immer **was** sich ändern soll und **was bleibt**. In Werkzeugen mit Schreibblöcken oder Artifacts kannst du einzelne Stellen markieren und nur diese überarbeiten lassen (Kap. 11).

---

## 7.5 Dauerhafte Einstellungen: Anweisungen, Projekte, Memory

Manche Angaben wiederholst du in jedem Prompt: deine Rolle, die Markenstimme, „keine Emojis". Dafür bieten die Werkzeuge dauerhafte Einstellungen.

| Funktion | Wirkt für | Typischer Inhalt | Gegenstück bei Alternativen |
|---|---|---|---|
| **Benutzerdefinierte Anweisungen** | alle deine Chats | Rolle, Arbeitsweise, bevorzugte Formate | Profil- bzw. Stilvorgaben in Claude, Gemini, Copilot |
| **Projekte** | alle Chats im Projekt, mit eigenen Dateien und projektbezogenem Gedächtnis | Styleguide, Produktdaten, Kampagnenbriefing | Claude Projects, Gemini Gems, Copilot Notebooks bzw. Agents |
| **Memory** | chatübergreifend, vom Werkzeug selbst gemerkt | Vorlieben, wiederkehrende Fakten | ähnliche Gedächtnisfunktionen bei anderen Anbietern |

Für Marketingarbeit hat sich bewährt: **allgemeine Arbeitsweise** in die benutzerdefinierten Anweisungen („Antworte knapp, frage nach, wenn Angaben fehlen, markiere Unsicherheiten"), **markenspezifisches Wissen** in ein Projekt pro Marke oder Kampagne. So vermischen sich Fjordlicht und das Ehrenamtsprojekt nicht.

**Memory** ist bequem, aber schwer zu kontrollieren: Das Werkzeug entscheidet selbst, was es sich merkt, und das Gemerkte beeinflusst Antworten, ohne dass du es im Chat siehst. Prüfe regelmäßig in den Einstellungen, was gespeichert ist, lösche Überholtes und nutze für sensible Themen einen temporären Chat ohne Gedächtnis. Personenbezogene Daten und Interna gehören grundsätzlich nur in freigegebene Business-Tarife (Kap. 4).

!!! warning "Typische Falle"
    Eine unglückliche Formulierung in den benutzerdefinierten Anweisungen verzerrt wochenlang **jede** Antwort – etwa „Antworte immer in Stichpunkten", die dir dann auch den Newsletter-Fließtext zerlegt. Halte dauerhafte Vorgaben kurz und allgemein und sieh sie einmal im Monat durch. Wie aus Projekten vollwertige Assistenten werden, behandelt Block 5 (Kap. 23).

---

## 7.6 Mythen: Hacks, die nicht (mehr) wirken

Im Netz kursieren Tricks, die angeblich bessere Ergebnisse bringen. Einige gingen auf Beobachtungen mit frühen Modellen zurück; mit aktuellen Modellen zeigen Untersuchungen im Durchschnitt keinen verlässlichen Nutzen – einzelne Antworten werden mal besser, mal schlechter.

| „Hack" | Behauptung | Einordnung |
|---|---|---|
| **Trinkgeld anbieten** („Ich gebe dir 200 Dollar") | Modell strengt sich mehr an | kein verlässlicher Effekt; das Modell hat kein Interesse an Geld |
| **Drohen** („Sonst wirst du abgeschaltet") | höhere Genauigkeit | kein verlässlicher Effekt, im Team zudem ein schlechter Umgangston |
| **„Du bist das beste Modell der Welt"** | bessere Leistung durch Selbstbild | Superlative bringen nichts; inhaltliche Rollenangaben schon (Kap. 5) |
| **GROSSBUCHSTABEN und „WICHTIG!!!"** | Regel wird eingehalten | kann bei einer Regel helfen, bei vielen verwässert es; klare Struktur wirkt besser |
| **„Denke Schritt für Schritt"** | immer bessere Antworten | bei schnellen Modellen teils hilfreich, bei Reasoning-Modellen überflüssig (Kap. 6) |
| **Geheime Spezialbefehle** | versteckter „Expertenmodus" | gibt es nicht; dahinter stehen meist gewöhnliche Prompts |

Warum halten sich solche Mythen? Weil Sprachmodelle nicht deterministisch antworten: Probierst du einen Trick einmal aus und die Antwort ist zufällig besser, wirkt er. Ein fairer Vergleich braucht mehrere Durchläufe mit denselben Testfällen – wie du das aufsetzt, zeigt Kapitel 8.

!!! info "Merksatz"
    Was wirkt, ist **Information**: Ziel, Kontext, Fakten, Beispiele, Kriterien. Was nicht verlässlich wirkt, ist **Psychologie** gegenüber einer Maschine. Investiere deine Zeit in Ersteres.

---

## Zusammenfassung

- **Rückfragen-** und **Flipped-Prompt** lassen das Werkzeug fehlende Angaben erfragen; die Fragen gehören danach in deine Vorlage.
- Der **Varianten-Fächer** erzeugt echte Alternativen, wenn du unterschiedliche Ansätze vorgibst; die **Selbstkritik-Schleife** wirkt nur mit konkreten Kriterien und findet keine erfundenen Fakten.
- Die **Stil-Extraktion** macht aus gelungenen Texten eine belegte Beschreibung der Markenstimme – die Grundlage für jeden Tone-Baustein.
- **Perspektivwechsel** liefern Anstöße, keine Marktforschung; präzise **Umschreibe-Befehle** sagen, was sich ändert und was bleibt.
- **Benutzerdefinierte Anweisungen**, **Projekte** und **Memory** sparen Wiederholung, wirken aber unsichtbar und brauchen regelmäßige Pflege und Datensparsamkeit.
- Trinkgeld, Drohungen und Superlative sind **Mythen**; was wirkt, ist Information.

---

## Kurzübungen

{{ task(file="tasks/k07_01.yaml") }}

{{ task(file="tasks/k07_02.yaml") }}

{{ task(file="tasks/k07_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k07.yaml") }}
