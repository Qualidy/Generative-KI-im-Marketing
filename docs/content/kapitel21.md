# Kapitel 21 – SEO mit KI I: Keyword-Recherche und Content-Briefing

{{ progress(21) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Warum die **Suchintention** wichtiger ist als das einzelne Keyword
- Wie du mit KI **Keyword-Ideen** sammelst und zu **Themenclustern** ordnest
- Wo die **Grenze** liegt: Warum KI keine Suchvolumina kennt und welche **Tools** diese Lücke schließen
- Wie du eine **Themenrecherche** mit Suchergebnisseite, Konkurrenz und Kundenfragen aufbaust
- Wie du aus allem ein **SEO-Briefing** erstellst, mit dem Mensch oder KI einen Text schreiben kann
</div>

---

## 21.1 SEO im Jahr 2026: Was sich geändert hat und was nicht

Suchmaschinenoptimierung (SEO) heißt: Inhalte so gestalten, dass Menschen sie über Suchmaschinen finden – und dass sie dort die Antwort bekommen, die sie suchen. Daran hat sich im Kern nichts geändert. Geändert hat sich die Umgebung: Google zeigt bei vielen Suchanfragen **AI Overviews**, also KI-Zusammenfassungen über den klassischen Ergebnissen, und bietet mit dem **AI Mode** einen dialogischen Suchmodus an. Gleichzeitig suchen viele Menschen direkt in ChatGPT, Perplexity oder Gemini. Was das für die Optimierung bedeutet, behandelt Kap. 22.

Für die Recherche gilt: KI ist ein hervorragender **Ideengeber und Ordner**, aber eine schlechte **Datenquelle**. Sie kann in Minuten hundert Suchbegriffe rund um „Regenjacke" vorschlagen, nach Absicht sortieren und zu Clustern bündeln. Sie kann dir aber nicht verlässlich sagen, wie oft „Regenjacke Damen nachhaltig" im Monat gesucht wird. Dieses Kapitel trennt beides sauber.

!!! info "Merksatz"
    KI liefert **Ideen und Struktur**, SEO-Tools liefern **Zahlen**. Wer Suchvolumina von einem Chatbot übernimmt, plant auf Sand.

---

## 21.2 Suchintention: Was will die Person eigentlich?

Hinter jeder Suchanfrage steckt eine Absicht. Google versucht, genau diese Absicht zu bedienen – ein Text, der die falsche Absicht trifft, rankt kaum, egal wie gut er geschrieben ist. Man unterscheidet üblicherweise vier Typen:

| Suchintention | Was die Person will | Beispiel Fjordlicht | Passender Inhalt |
|---|---|---|---|
| Informational | etwas wissen oder verstehen | „Wassersäule Regenjacke erklärt" | Ratgeber im Blog „Draußen-Notizen" |
| Navigational | eine bestimmte Seite finden | „Fjordlicht Sølv" | Produktseite, Startseite |
| Kommerziell (Commercial) | Optionen vergleichen vor dem Kauf | „nachhaltige Regenjacke Test" | Kaufberatung, Vergleich, Materialerklärung |
| Transaktional | jetzt kaufen oder handeln | „Regenjacke Damen kaufen" | Kategorieseite im Shop |

Die einfachste Prüfung der Intention: **Schau dir die Suchergebnisseite an.** Wenn bei „Regenjacke waschen" nur Ratgeber und Videos erscheinen, wird eine Produktseite dort nicht ranken. KI kann die Intention gut einschätzen, aber sie sieht die aktuelle Ergebnisseite nur, wenn du die Websuche aktivierst oder die Ergebnisse selbst einfügst.

!!! warning "Typische Falle"
    Ein Keyword, ein Text – und alle vier Intentionen sollen bedient werden. Ein Blogartikel, der gleichzeitig erklärt, vergleicht und verkauft, wirkt wie eine Werbebroschüre mit Ratgeber-Überschrift. Entscheide dich pro Seite für **eine** Hauptintention und verlinke für den nächsten Schritt auf die passende andere Seite.

---

## 21.3 Keyword-Ideen sammeln und clustern

Im ersten Schritt nutzt du die Stärke der KI: Breite. Ausgangspunkt sind **Seed-Keywords**, also die Grundbegriffe deines Themas („Regenjacke", „Outdoorjacke", „Wanderjacke"). Daraus lässt du Varianten ableiten: **Long-Tail-Keywords** (längere, spezifische Suchanfragen wie „Regenjacke für Radfahren in der Stadt"), W-Fragen, Synonyme und die Sprache der Zielgruppe.

Ein Prompt nach dem P.R.O.M.P.T.-Framework (Kap. 5) sieht so aus:

```text
Persona: Du bist SEO-Spezialistin für E-Commerce im Bereich Outdoor-Bekleidung.
Request: Sammle Suchbegriffe rund um das Thema "Regenjacke", die Menschen
in Deutschland bei Google eingeben könnten. Ordne sie anschließend in
Themencluster.
Output: Tabelle mit den Spalten Cluster, Suchbegriff, vermutete Suchintention
(informational, navigational, kommerziell, transaktional), passender Seitentyp.
Mindestens 40 Begriffe, 5 bis 8 Cluster.
Modifier: Nenne KEINE Suchvolumina oder Schwierigkeitswerte, du kennst sie
nicht. Berücksichtige Alltagssprache und Fragen ("wie", "was", "welche").
Keine Markennamen von Wettbewerbern.
Purpose: Grundlage für die Content-Planung des Blogs und der Kategorieseiten
von Fjordlicht, einer nachhaltigen Outdoor-Marke; Zielgruppe naturverbundene
Stadtmenschen 25 bis 45 und Familien.
Tone: sachlich, keine Kommentare zwischen den Tabellen.
```

Das Ergebnis ist eine geordnete Rohliste. Typische Cluster wären „Pflege und Imprägnierung", „Material und Technik", „Kaufberatung", „Regenjacke für Kinder", „Nachhaltigkeit". Jedes Cluster kann zu einer **Pillar Page** (umfassende Übersichtsseite) mit mehreren verlinkten Detailartikeln werden – dieselbe Logik wie bei den Content-Pillars im Redaktionsplan (Kap. 12).

Bewährt hat sich, die Sammlung als **Prompt-Kette** (Kap. 6) in mehreren Schritten anzulegen statt in einem einzigen Riesenprompt: erst breit sammeln, dann Dubletten und Kunstbegriffe streichen lassen, dann clustern, zuletzt jedem Cluster einen Seitentyp zuordnen. Nach jedem Schritt prüfst du kurz selbst. So bemerkst du früh, wenn die KI in eine Richtung abdriftet – etwa nur noch Fachbegriffe wie „Laminat" und „Membrantechnologie" liefert, die eine Familie bei der Suche nach einer Kinderregenjacke nie eintippen würde. Frag zur Kontrolle ausdrücklich: „Welche dieser Begriffe würde ein Mensch ohne Fachwissen tatsächlich so in die Suche eingeben?"

!!! tip "Die Sprache der Kundschaft einbauen"
    Die besten Long-Tail-Ideen kommen nicht aus dem Modell, sondern aus echten Fragen: Kundenservice-Mails, Produktbewertungen, Kommentare unter Posts, Ergebnisse aus dem Social Listening (Kap. 19). Gib der KI eine anonymisierte Liste solcher Fragen und lass sie daraus Suchbegriffe ableiten. Das Ergebnis ist deutlich näher an der Wirklichkeit als ein reines Brainstorming.

---

## 21.4 Die Grenze: KI kennt keine Suchvolumina

Sprachmodelle haben keinen Zugriff auf die Suchdaten von Google. Fragst du nach Suchvolumen oder Keyword-Schwierigkeit, bekommst du trotzdem oft Zahlen – plausibel klingend, sauber formatiert und **erfunden** (Kap. 2). Auch mit aktivierter Websuche findet das Modell höchstens veraltete Werte aus Blogartikeln. Für die Priorisierung brauchst du deshalb Daten aus Werkzeugen, die auf echten Suchdaten oder großen Panels beruhen:

| Werkzeug | Was es liefert | Hinweis |
|---|---|---|
| Google Keyword Planner | Suchvolumen-Schätzungen, verwandte Begriffe | Teil von Google Ads; ohne laufende Kampagnen oft nur Spannen |
| Google Search Console | echte Impressionen, Klicks, Position für deine eigene Website | nur für Begriffe, bei denen du schon sichtbar bist |
| Google Trends | relative Entwicklung und Saisonalität | keine absoluten Zahlen |
| Sistrix, Semrush, Ahrefs u. ä. | Suchvolumen, Schwierigkeit, Wettbewerber-Keywords | kostenpflichtig, Werte sind Schätzungen und weichen voneinander ab |
| „Ähnliche Fragen" in der Google-Suche | echte Anschlussfragen | manuell auswerten oder per Tool exportieren |

Der sinnvolle Ablauf ist ein Wechselspiel: Die KI erzeugt und ordnet Ideen, das Tool liefert Zahlen, die KI hilft beim Priorisieren. Dazu exportierst du die Tool-Daten als Tabelle und lädst sie mit deinen Clustern hoch – ab dann arbeitet die KI mit echten Werten.

!!! warning "Typische Falle"
    Die Frage „Wie hoch ist das Suchvolumen?" wird oft beiläufig gestellt, und die KI antwortet beiläufig mit einer Zahl. Schreibe deshalb in jeden Keyword-Prompt den Modifier „Nenne keine Suchvolumina" und prüfe jede Zahl in einer Tabelle auf ihre Herkunft. Eine Zahl ohne Quelle gehört gestrichen.

Für Fjordlicht ist die **Search Console** der wertvollste Startpunkt: Sie zeigt Suchbegriffe, für die der Blog schon auf Position 8 bis 20 erscheint. Diese „Fast-Treffer" lassen sich mit überschaubarem Aufwand verbessern – Thema der Bestandsoptimierung in Kap. 22.

---

## 21.5 Themenrecherche: Ergebnisseite, Konkurrenz, Lücken

Steht das Keyword, prüfst du, was zum Thema bereits gut rankt. Diese **SERP-Analyse** (Search Engine Results Page) beantwortet drei Fragen: Welche Inhaltsformen erscheinen (Ratgeber, Video, Shop, Forum)? Welche Unterthemen behandeln die vorderen Ergebnisse? Was fehlt überall?

Hier ist KI ein guter Analysepartner, wenn du ihr Material gibst. Mit aktivierter Websuche oder Deep Research kann sie aktuelle Seiten selbst lesen; zuverlässiger ist es, die Gliederungen der fünf besten Ergebnisse zu kopieren und einzufügen.

```text
Hier sind die Zwischenüberschriften der fünf bestplatzierten Artikel zu
"Regenjacke imprägnieren" (getrennt durch ###).
###
[Gliederungen einfügen]
###
1. Welche Unterthemen kommen in mindestens drei Artikeln vor?
2. Welche Fragen bleiben in allen Artikeln unbeantwortet?
3. Wo könnte Fjordlicht mit eigener Erfahrung (Reparaturservice,
   Materialtests) etwas bieten, das die anderen nicht haben?
Antworte in drei kurzen Listen.
```

Bei Deep Research gilt dieselbe Vorsicht wie bei jeder Websuche (Kap. 9): Das Werkzeug fasst gefundene Seiten zusammen, sieht aber nicht unbedingt dieselbe Ergebnisseite wie deine Kundin, und es kann Inhalte falsch zuordnen. Öffne die zwei, drei wichtigsten Quellen deshalb selbst.

Frage 3 ist die wichtigste. Inhalte, die nur zusammenfassen, was schon rankt, haben wenig Chance – und sind genau die Art Text, die KI ohnehin massenhaft erzeugen kann. Der Vorsprung entsteht durch **Erfahrung** und eigene Daten: Fjordlicht weiß aus dem Reparaturservice, welche Imprägnierfehler am häufigsten vorkommen. Das ist die „Experience" in E-E-A-T (Kap. 15).

!!! example "Content-Gap bei Fjordlicht"
    Die Analyse zeigt: Alle Top-Artikel erklären Sprühimprägnierung und Waschimprägnierung, keiner beantwortet, wie man erkennt, ob die Membran oder nur die Außenimprägnierung nachlässt. Fjordlicht kann das mit Fotos aus der eigenen Werkstatt erklären – ein echtes Alleinstellungsmerkmal.

---

## 21.6 Das SEO-Briefing

Das **SEO-Briefing** bündelt die Recherche in einem Dokument, mit dem ein Mensch, eine Agentur oder die KI einen Text schreiben kann. Es ist die Brücke zur Texterstellung in Kap. 15 und zur On-Page-Optimierung in Kap. 22.

| Feld | Inhalt am Beispiel „Regenjacke imprägnieren" |
|---|---|
| Hauptkeyword | Regenjacke imprägnieren |
| Nebenkeywords | Regenjacke waschen, Imprägnierung erneuern, Jacke perlt nicht mehr ab |
| Suchintention | informational |
| Zielgruppe | Besitzer:innen einer Funktionsjacke, die nicht mehr dicht wirkt |
| Ziel der Seite | Pflegeanleitung, danach Link zum Reparaturservice und zur Sølv |
| Kernfragen | Wann imprägnieren? Wie? Welches Mittel? Membran oder Imprägnierung? |
| Alleinstellung | Erfahrungen aus der Fjordlicht-Werkstatt, Fehlerbilder mit Fotos |
| Gliederungsvorschlag | H2-Struktur aus der SERP-Analyse plus Lücke |
| Umfang | Richtwert aus Konkurrenzanalyse, kein Selbstzweck |
| Interne Links | Pflege-Pillar, Produktseite Sølv, Reparaturservice |
| Markenstimme und No-Gos | ruhig, ehrlich, keine Superlative, nur belegbare Umweltaussagen |

Die KI kann dieses Briefing aus deinen Rechercheergebnissen entwerfen. Gib ihr dazu Keyword-Tabelle mit Tool-Daten, SERP-Analyse und Styleguide und fordere ausdrücklich, Felder ohne Grundlage mit `[OFFEN]` zu markieren. Der Mensch ergänzt dann Alleinstellung und Ziel – die beiden Felder, die keine KI kennen kann.

```mermaid
flowchart LR
    A([Seed-Keywords]) --> B([KI: Ideen und Cluster])
    B --> C([Tool: Volumen und Daten])
    C --> D([SERP-Analyse und Lücken])
    D --> E([SEO-Briefing])
    E --> F([Text erstellen Kap. 15])
```

!!! tip "Briefing als Bibliotheksvorlage"
    Lege die Briefing-Felder als Vorlage in eurer Prompt-Bibliothek ab (Kap. 10). So entsteht jedes Briefing in derselben Struktur, und Texte aus verschiedenen Händen bleiben vergleichbar.

---

## Zusammenfassung

- SEO bleibt das Bedienen von **Suchabsichten**; neu ist die Umgebung mit AI Overviews und KI-Suche (Kap. 22).
- Die **Suchintention** (informational, navigational, kommerziell, transaktional) entscheidet über den Seitentyp – prüfe sie an der Ergebnisseite.
- KI eignet sich hervorragend zum **Sammeln und Clustern** von Keywords, besonders mit echten Kundenfragen als Input.
- KI kennt **keine Suchvolumina**: Zahlen kommen aus Keyword Planner, Search Console, Trends oder Sistrix/Semrush.
- Die **SERP-Analyse** zeigt, was schon rankt; der Vorsprung entsteht durch eigene Erfahrung und Lücken.
- Das **SEO-Briefing** bündelt Keyword, Intention, Ziel, Gliederung und Alleinstellung als Grundlage für jeden Text.

---

## Kurzübungen

{{ task(file="tasks/k21_01.yaml") }}

{{ task(file="tasks/k21_02.yaml") }}

{{ task(file="tasks/k21_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k21.yaml") }}
