# Feedback-Coach – ein Claude-Skill für bessere Feedback-Gespräche

Der Feedback-Coach ist ein Skill für [Claude](https://claude.ai). Er hilft dir, Feedback klar, fair und umsetzbar zu formulieren, egal ob an Mitarbeitende, Kolleg:innen, die eigene Führungskraft oder im privaten Umfeld.

Der Coach schreibt dein Feedback **nicht** für dich. Er stellt dir Fragen, eine nach der anderen, bis du selbst eine Formulierung gefunden hast, die zu dir und zur Situation passt.

## Was der Coach kann

Er arbeitet in drei Modi:

- **Vorbereiten:** Du gehst ein echtes Gespräch Schritt für Schritt durch: Situation, konkretes Verhalten, Wirkung, deine Erwartung, der nächste Schritt und eine offene Frage an dein Gegenüber.
- **Entwurf prüfen:** Du bringst einen fertigen Text mit. Der Coach zeigt dir, was schon gut funktioniert und wo du nachschärfen kannst, jeweils mit einer Frage, statt dir eine fertige Fassung zu liefern.
- **Üben:** Du trainierst an Übungsfällen auf Deutsch oder Englisch, vom Einstieg (konkretes Lob) bis fortgeschritten (Konflikt zwischen zwei Teammitgliedern). Danach siehst du typische Fallen und eine Beispielantwort.

Unterwegs achtet der Coach darauf, ob du dem eigentlichen Thema ausweichst, zum Beispiel durch Kleinreden, viel Lob drumherum oder ein Gespräch ohne festen Termin, und spricht das freundlich an.

Auf Wunsch protokolliert er jede Sitzung kurz, etwa in einem Google Doc oder in Notion, ohne Namen und mit einer Legende, damit die Einträge auch später noch verständlich sind. Beim nächsten Mal knüpft er daran an.

## Worauf er sich stützt

Das Gespräch folgt dem Praxismodell **SBI** (Situation – Verhalten – Wirkung) als Struktur. Ob ein Feedback gut ist, entscheidet ein Regelwerk aus der Feedback-Forschung, unter anderem:

- Kluger & DeNisi (1996): Feedback, das auf die Person statt auf die Aufgabe zielt, verschlechtert die Leistung oft sogar.
- Hattie & Timperley (2007): vier Ebenen von Feedback sowie Feed Up, Feed Back und Feed Forward.
- Goodman, Wood & Hendrickx (2004): Zu detailliertes Feedback bremst eigenständiges Lernen.
- Ilgen, Fisher & Taylor (1979): Feedback wirkt nur, wenn es akzeptiert wird, und beobachtbares Verhalten ist glaubwürdiger als Deutungen.
- Kluger & Nir (2010): das Feedforward-Interview.

Die vollständige Literaturliste steht in der [`SKILL.md`](feedback-coach/SKILL.md). Im Gespräch bleibt die Theorie im Hintergrund. Der Coach spricht Alltagssprache und nennt Quellen nur, wenn du danach fragst.

## Was er bewusst nicht tut

- Er schreibt dein Feedback nicht für dich.
- Er bewertet keine Menschen und keine Leistung und bereitet keine Beurteilungen, Abmahnungen oder Kündigungen vor. Dafür sind HR, Führungskraft oder Betriebsrat die richtigen Ansprechpartner.
- Bei Belästigung, Diskriminierung, Gewalt oder einer psychischen Krise ist ein Feedback-Gespräch nicht der richtige Weg. Dann verweist der Coach auf passende Anlaufstellen.
- Er ersetzt keine Beziehung und kein Vertrauen. Er verbessert die Vorbereitung und die Formulierung, nicht die Haltung.

**Datenschutz:** Lass Namen und Details weg, an denen man Personen erkennen könnte. „Die Kollegin“ oder „mein Teamleiter“ reicht völlig.

## Installation in Claude

1. Lade die Datei [`feedback-coach.zip`](feedback-coach.zip) aus diesem Repo herunter, oder pack den Ordner `feedback-coach` selbst als ZIP. Wichtig: Der Ordner muss in der ZIP-Datei ganz oben liegen, nicht nur die `SKILL.md`.
2. Öffne in Claude **Plugins > Skills** und lade dort die ZIP-Datei hoch.
3. Achte darauf, dass der Skill eingeschaltet ist.

**Alternative ohne ZIP:** Nutze in Claude den Skill-Builder-Skill und gib ihm den Inhalt der [`SKILL.md`](feedback-coach/SKILL.md). Er legt den Skill dann für dich an.

Die Menüs in Claude ändern sich ab und zu. Falls du die Stelle nicht findest, hilft die [Hilfe von Anthropic](https://support.claude.com/en/articles/12512180-using-skills-on-claude-ai) weiter.

Skills sind in allen Claude-Tarifen verfügbar, setzen aber voraus, dass Code-Ausführung aktiviert ist.

## Nutzung mit anderen KI-Assistenten

Der Skill ist nicht an Claude gebunden. Die `SKILL.md` ist eine normale Textdatei mit Anweisungen, und die funktionieren auch mit anderen KI-Assistenten:

- **Mit Skill-Funktion:** Einige Assistenten, zum Beispiel Gemini, unterstützen inzwischen ebenfalls Skills. Dort kannst du die `SKILL.md` oder die ZIP-Datei ähnlich einbinden wie in Claude.
- **Ohne Skill-Funktion:** Frag deine KI einfach, wie du die `SKILL.md` am besten mit ihr teilst, damit sie die Anweisungen dauerhaft nutzt, zum Beispiel als eigener Assistent, in den Projekt-Anweisungen oder als hochgeladene Datei zu Beginn eines Chats.

Ein paar Details im Skill sind auf Claude zugeschnitten, etwa das Speichern der Sitzungsprotokolle über verbundene Apps. Das Coaching selbst funktioniert auch ohne diese Funktionen.

## Loslegen

Schreib Claude zum Beispiel:

- „Ich will meiner Kollegin Feedback geben.“
- „Kannst du meinen Feedback-Entwurf prüfen?“
- „Ich möchte Feedback-Gespräche üben.“

## Webseite

Das Repo enthält eine Webseite (`index.html`), die den Coach für alle ohne Technik-Hintergrund erklärt. Dort kann man den kompletten Coach mit einem Klick kopieren und in jede KI einfügen, oder den Skill herunterladen.

Die Seite läuft über GitHub Pages: Unter **Settings > Pages** bei „Source“ **Deploy from a branch** wählen, dann den Branch `main` und den Ordner `/ (root)` einstellen und speichern. Nach ein bis zwei Minuten ist sie unter `https://<dein-name>.github.io/feedback-coach/` erreichbar. Die leere Datei `.nojekyll` sorgt dafür, dass die `SKILL.md` unverändert ausgeliefert wird. Sie darf nicht gelöscht werden.

## Lizenz

MIT, siehe [`LICENSE`](LICENSE). Du darfst den Skill nutzen, anpassen und weitergeben.
