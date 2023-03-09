# Erstes Node

Der Godot Editor ist gestartet und hat dein erstes eigenes Projekt geöffnet. Du kannst den Namen deines Projekts oben in der Titelleiste sehen.

![Der Godot Editor mit geöffnetem Projekt]()

!!! tip "Die erste Hürde nehmen: Einfach loslegen!"
    Ein leeres Projekt ist vergleichbar mit einem leeren Blatt Papier, wenn man einen Text schreiben oder ein Bild malen will: Man weiß nicht genau, wie man anfangen soll, weil irgendwie kommen die Ideen erst, wenn man schon mittendrin ist. Um in einen solchen "Fluss" zu kommen (und das gilt für alle kreativen Tätigkeiten), gibt es eine einfache Hilfe:

    Erstelle bei einem neuen Projekt zu Beginn immer etwas ganz Kleines und schaue es dir an, als wäre dein Projekt damit schon fertig. Du erhälst sofort ein Ergebnis - und das mit minimalem Aufwand. Dies motiviert und gibt dir einen Schubs, Stück für Stück mehr hinzuzufügen.

    Das funktioniert in der Godot Engine super, weil du hier schrittweise vorgehen kannst (das nennt man auch _iterativ_) und du nicht von Anfang bis Ende alles vorher durchdenken musst. 

Auf der linken Seite findest du oben den `Scene-Dock`. Dort steht _Create Root Node_ und darunter findest du vier Buttons: 2D Scene, 3D Scene, User Interface und Other Node.

![Der Szenen-Dock]()

Klicke auf `2D Scene`, denn wir wollen ein 2D-Programm erstellen. Nun ändert sich der `Scene-Dock` und es steht dort nur noch `Node2D`. Weiterhin hat sich in der Mitte des Editors der sogenannte `Viewport` automatich auf die 2D-Ansicht umgestellt.

![Editor mit 2D-Szene]()

!!! question "Scene? Node? Was ist das?"
    Diese beiden Begriffe sind zwei der Kernelemente von Godot. Im Detail wirst du sie erst nach und nach verstehen, aber für den Anfang kann man es sich wie folgt vorstellen:

    Ein Spiel ist wie ein Theaterstück: Es gibt eine Bühne und auf dieser gibt es Schauspieler, einen Hintergrund, allerlei Gegenstände und irgendwo sitzt noch ein Orchester für die Musik - diese Grundelemente sind im übertragenen Sinne unsere **Nodes**.
    Ein solches Theaterstück ist in **Szenen** unterteilt, bei denen die Bühne jeweils anders aufgebaut ist: ein anderer Hintergrund, andere Schauspieler und Gegenstände (welche aber auch wiederverwendet werden können). Unsere **Scenes** bestehen also aus verschiedenen **Nodes** und diese ergeben ein Gesamtbild, welches das Spiel ausmacht.

Die Szene heißt aktuell noch `Node2D`. Da es sich um die Hauptszene in deinem Programm handelt, kannst du sie bspw. umbenennen in `Main`. Klicke dazu im `Scene`-Dock mit Rechtsklick auf das Node `node2D` und wähle dort den Eintrag `Rename` (du kannst auch nach dem Klick auf das Node die Taste F2 drücken). Nun kannst du `Main` eingeben und mit Enter bestätigen.

Klicke nun oben in der Menüleiste auf `Scene` und dort auf `Save Scene` (du kannst auch einfach ++"Strg"+s++ drücken).

![Menüleiste mit Szene speichern]()

Im daraufhin geöffneten Dialog bist du automatisch im Pfad `res://`. Dies ist dein Ressourcenordner, welcher deinem zuvor gewählten Projektordner entspricht. Aktuell hast du noch keine Szenendateien oder Unterordner in deinem Projekt, deswegen wird dir ein leeres Fenster angezeigt. Am unteren Rand kannst du den vorgeschlagegen Dateinamen `main.tscn` sehen. Belasse ihn so und drücke rechts unten auf `Save`.

!!! question "Was ist eine tscn-Datei?"
    Szenen werden als sogenannte PackedScene verpackt und dann im Dateisystem als tscn-Datei gespeichert. Dieser Dateityp kann nur mit der Godot Engine geöffnet und bearbeitet werden. (Mir ist zumindest kein anderes Programm bekannt, was das könnte.)

Nach dem Speichern siehst du unten links im `FileSystem`-Dock neben der `icon.svg`-Datei jetzt deine `main.tscn`-Datei.

![FileSystem-Dock mit main.tscn]()

Klicke nun oben rechts im Godot Editor bei den sogenannten Playtest-Buttons auf ▶️ Play, um das gesamte Projekt zu starten.

![Playtest Buttons]()

Es wird eine Meldung angezeigt, dass noch keine Hauptszene ausgewählt wurde. Die Hauptszene eines Projekts, wird beim Start als erstes geladen und angezeigt. Klicke hier auf den Button `Select current`, um die aktuelle `Main`-Scene auszuwählen.

![Main-Scene Dialog]()

Es öffnet sich nun ein neues Fenster mit einem grauen Hintergrund. In der Titelleiste sollte der Name deines Projektes stehen und dahinter _(DEBUG)_. Das Fenster kann verkleiner, vergrößert, minimiert und maximiert werden und zeigt aber immer einen grauen Hintergrund. Mehr passiert nicht. Schließe das Fenster mit einem Klick auf das X (du kannst auch die Taste ++f8++ drücken).

![Playtest Debugfenster]()

Damit hast du einen großen Sprung gemacht! Du hast nicht nur ein eigenes Projekt angelegt und deine erste Szene mit einem ersten Node darin erstellt. Nein, du hast auch noch dein Programm zum ersten Mal gestartet und es wurde ein Fenster angezeigt. Am Ende also so wie bei einem richtigen Spiel!
