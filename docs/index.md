# Spieleprogrammierung mit der Godot Engine - Ein Workshop bei den Chemnitzer Linux-Tagen

## Intro

!!! info "Ein freundliches Hallo"
	Herzlich willkommen!
	
	Diese Seite dient der Begleitung von Workshops zum Thema Godot. Du kannst sie aber auch durcharbeiten, ohne einen Workshop zu besuchen.
	Ich wünsche dir jedenfalls viel Spaß bei der Lektüre. Hier und da fehlt sicherlich noch etwas, aber lass dich davon nicht aufhalten. Bei Fragen kannst du einfach bei GitHub einen [Diskussionsbeitrag](https://github.com/pwab/godot-clt-workshop/discussions) erstellen!
	
	*Viele Grüße<br>
	\- Philipp*
	
	![pwab beim CLT-Adventure](assets/index/pwab_cltadventure.png)

Godot ist eine freie Spiel-Engine, mit der sich auf einfache Weise Ideen für Spiele und Apps auf PC, Smartphone oder im Webbrowser umsetzen lassen. Der Einstieg ist überraschend einfach und viele Sachen sind schnell gemacht. Im Workshop wird die Godot Engine vorgestellt. Unter Anleitung werden Spielelemente wie Animationen, Sound und Kollisionen für ein kleines 2D-Spiel Schritt für Schritt eingebaut und Fallstricke dabei erklärt. Am Ende des Workshops sollen die Teilnehmer gesehen haben, wie die Godot Engine aufgebaut ist und wie man damit die einzelnen Grundbausteine eines Spiels nach und nach zusammenfügt. Da man in einem solchen Kurs trotz des zeitlichen Umfangs nur an der Oberfläche der Spieleentwicklung kratzen kann, gibt es online weiterführendes Kursmaterial, mit dessen Hilfe man sich dann selbstständig weitere Themen erarbeitet kann.

## Voraussetzungen

Der Workshop ist konzipiert für Jugendliche etwa ab der 8. Klasse. Programmierkenntnisse sind nicht notwendig, da im Laufe des Workshops alle Codeteile gezeigt und erläutert werden. Der Kurs wird auf Deutsch gehalten, der Code wird allerdings auf Englisch geschrieben, da dies im Programmierbereich üblich ist. Dafür sind jedoch nur grundlegende Sprachkenntnisse notwendig und alle Programmteile werden beim Einfügen auf Deutsch erklärt.

Eine Teilnahme ist auch für andere Personengruppen (bspw. jüngere Kinder unter Begleitung eines Erwachsenen oder ältere/erfahrenere Jugendliche) möglich. Allerdings kann hier nicht auf die speziellen Bedürfnisse (bspw. Über- oder Unterforderung) eingegangen werden - ich werde dennoch mein Bestes versuchen.

Die benötigte Software ist für alle gängigen Betriebssysteme verfügbar und dank einer Größe von knapp 40 MB schnell heruntergeladen. Eine Installation wird in der Regel nicht benötigt. Für die Teilnahme am Workshop wird ein PC mit Maus und Tastatur empfohlen, welcher OpenGL 2.1 / OpenGL ES 2.0 kompatible Hardware besitzt - das unterstützen heutzutage aber nahezu alle Rechner also keine Sorge. Zur Not gibt es auch einen [Webeditor](https://editor.godotengine.org/releases/latest/), welcher auf Tablets funktionieren könnte.

## Letzte Worte zur Vorbereitung

Also hier noch einmal als Checkliste zusammengefasst, was du zum Live-Workshop vorbereiten solltest:

- [x] Bring deinen Laptop mit (Betriebssystem ist egal)
- [ ] Optional: Bring einen Gamecontroller mit, der an deinem Laptop funktioniert (bspw. XBox oder PS-Controller)
- [ ] Lies das Kapitel zur [Einführung](introduction/01_welcome-structure.md)
- [ ] [Installiere](introduction/04_installation.md) die Godot Engine

Und falls der Workshop online stattfindet:

- [x] Sitz gemütlich vor deinem PC/Laptop (Tipp: Zwei Monitore helfen dabei, das Gesehene gleich mit umzusetzen)
- [x] Halte ein Headset mit Kopfhörern und am besten mit Mikrofon bereit (Zur Kommunikation wird es während des Workshops einen Textchat geben. Wer ein Mikrofon hat, kann auch dieses für das Stellen von Fragen nutzen. Eine Kamera wird nicht benötigt.)
- [x] Räume deinen Desktop auf, damit dieser nur Dinge zeigt, die öffentlich sichtbar sein dürfen, da wir eventuell den Bildschirm teilen, um einander zu helfen
- [ ] Lies das Kapitel zur [Einführung](introduction/01_welcome-structure.md)
- [ ] [Installiere](introduction/04_installation.md) die Godot Engine

!!! tip "Im Brandfall: Scheibe _nicht_ einschlagen!"
	Sollte etwas schieflaufen oder solltest du aus irgendwelchen Gründen nicht am Workshop teilnehmen können: **Keine Panik!**
	
	Auf dieser Webseite findest du alle Inhalte und Schritt-für-Schritt-Anleitungen zu den Themen des Workshops. Du kannst also jederzeit dir die Sachen selbstständig anschauen und den Workshop so nachholen.

## Weiterführende Links

- [Webseite der Chemnitzer Linux-Tage](https://chemnitzer.linux-tage.de/)
- [Offizielle Webseite der Godot Engine (Englisch)](https://godotengine.org/)
- [Source Code dieser Kurswebseite](https://github.com/pwab/godot-clt-workshop)

## Lizenz

![CC0 Lizenz Badge](assets/index/cc0_badge.png)

Der gesamte Workshopinhalt (Text, Bilder und Code) steht unter der [CC0-1.0](https://creativecommons.org/share-your-work/public-domain/cc0/) Lizenz. Er ist also frei nutzbar, kann ohne zu fragen kopiert, verändert und weitergegeben werden.

Eine Ausnahme bilden Screenshots, welche teilweise aus der offiziellen Dokumentation übernommen wurden (extra gekennzeichnet). Sie stehen - genauso wie das Godot Engine Logo - unter der [CC-BY-3.0](https://creativecommons.org/licenses/by/3.0/) Lizenz und wurden erstellt von _Juan Linietsky, Ariel Manzur and the Godot community_.