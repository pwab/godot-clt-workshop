# Erster Code

Damit mehr passiert, als dass nur ein Fenster angezeigt wird, müssen wir der Godot Engine sagen, was sie sonst noch so machen soll. Das machen wir durch Programmcode. Dieser wird in ein sogenanntes Skript geschrieben und dann entsprechend unserer Vorgaben von der Engine ausgeführt. Die Godot Engine bietet dazu die sehr einfache Programmiersprache **GDScript** an.

!!! info "GDScript"
    Die Diskussion, warum man für Godot eine neue Sprache lernen sollte, erspare ich mir hier. Lies dazu am besten einmal in der Dokumentation die Abschnitte zur [Design Philosophie](https://docs.godotengine.org/en/latest/getting_started/introduction/godot_design_philosophy.html) oder das [Intro zu den verfügbaren Skriptsprachen](https://docs.godotengine.org/en/latest/getting_started/step_by_step/scripting_languages.html).

    Für alle Neueinsteiger in die Programmierung kann ich GDScript wirklich wärmstens empfehlen. Wer zuvor bereits Erfahrung mit Python gesammelt hat, wird sich sofort wohl fühlen, denn diese beiden Sprachen sind sich sehr ähnlich.

Klicke im `Scene`-Dock mit der rechten Maustaste auf unser `Main`-Node und wähle `Attach Script`. 

![Rechtsklickmenü der Main-Node mit Attach Script]()

Es öffnet sich ein Dialog zum Erstellen eines Skriptes. Hier kann die Skriptsprache definieren, ein Template (also eine Vorlage) auswählen und den Pfad zum Abspeichern festlegen. Belasse einfach alle Voreinstellungen so wie sie sind. Im Textfenster am Ende wird angezeigt, was alles eingestellt ist und ob alle Einstellungen okay (= grün) sind. Klicke dann auf `Create` und das Skript wird als `main.gd` gespeichert.

!!! info "Was ist eine gd-Datei?"
    GD-Dateien sind einfache Textdateien, welche allerdings für die Godot Engine (und auch andere Editoren) sofort als GDScript-Codedateien erkannt werden.

![Dialog zur Skripterstellung]()

Und wieder passt sich der Godot Editor automatisch an und wechelt den Viewport in der Mitte zum Skripteditor. Die aktive Ansicht kannst du oben in der Mitte im Bereich der Menüleiste jederzeit ändern.

![Skripteditor mit Viewport-Ansichtsmenü]()

Unser Skript `main.gd` ist offenbar schon vorausgefüllt worden. Dies kommt daher, da wir die Einstellung zum Template bei der Skripterstellung belassen haben. Das beschleunigt enorm die Arbeit mit Skripten, denn man kann die voreingstellten Vorlagen der Godot Engine verwenden oder später auch eigene Vorlagen hinzufügen.

Schau dir die Vorlage einmal kurz an:

```gdscript title="Template" linenums="1"
extends Node2D


# Called when the node enters the scene tree for the first time.
func _ready():
	pass # Replace with function body.


# Called every frame. 'delta' is the elapsed time since the previous frame.
func _process(delta):
	pass

```

!!! abstract "Kurzerklärung zu den Zeilen der Vorlage"
    Hier nur eine grobe Übersicht über die einzelnen Zeilen des Skriptes:

    - `#!gdscript extends Node2D` ... Das Skript bezieht sich auf ein `Node2D`-Node und erhält (erbt) damit alle Eigenschaften und Methoden dieser Node.
    - `#!gdscript # Blabla` ... Ein Doppeklkreuz/Hashtag `#` leitet einen Kommentar ein.
    - `#!gdscript func _ready():` ... `func` leitet eine Funktion ein. Ein Unterstrich `_` ist die Kennzeichnung für Funktionen, welche von außen nicht aufgerufen werden können. Die `ready()`-Funktion ist eine vordefinierte Standardfunktion, welche aufgerufen wird, wenn das Node fertig geladen und bereit zur Anzeige ist. Die Funktion benötigt keine Parameter und hat deshalb leere Klammern `()`. Eine Funktionsdeklaration endet mit einem Doppelpunkt `:`.
    - `#!gdscript pass` ... Dies ist eine spezielle GDScript-Funktion die absolut nichts tut. Also wirklich gar nichts. Sie ist ein Platzhalter - in diesem Fall für den Funktionsinhalt.
    - `#!gdscript func _process(delta):` ... Die `process()`-Funktion ist eine vordefinierte Standardfunktion, welche dauerhaft in jedem Frame aufgerufen wird. Der Parameter `delta` gibt die Zeit zwischen dem letzten Frame und dem aktuellen Frame wieder und ermöglicht somit, dass man sich mit geschickter Programmierung von den FPS des Spielers unabhängig machen kann.

Im mittleren Teil findet man die `_ready()`-Funktion, welche beim Laden des Nodes, somit beim Laden der `Main`-Szene und somit schlussendlich also beim Starten des Programms aufgerufen wird:

```gdscript title="Template" linenums="1" hl_lines="5 6"
extends Node2D


# Called when the node enters the scene tree for the first time.
func _ready():
	pass # Replace with function body.


# Called every frame. 'delta' is the elapsed time since the previous frame.
func _process(delta):
	pass

```

Dort in Zeile 6 unter `#!gdscript func _ready():` entfernst du jetzt das `#!gdscript pass` und dann tippst du mit einem ++tab++ eingerückt die Zeile `#!gdscript print("Hello World")` ein. Der Abschnitt sollte also wie folgt aussehen:

```gdscript linenums="5"
func _ready():
    print("Hello World")
```

Hier ist zur Kontrolle noch einmal das gesamte Skript:

```gdscript title="Template" linenums="1" hl_lines="5 6"
extends Node2D


# Called when the node enters the scene tree for the first time.
func _ready():
    print("Hello World")


# Called every frame. 'delta' is the elapsed time since the previous frame.
func _process(delta):
	pass

```

Klicke in der Menüleiste des Skripteditors auf `File` und dann auf `Save` (oder drücke einfach ++"Strg"+s++). Nun kannst du wieder den Play-Button im Editor klicken (oder du drückst die Taste ++f5++).

Es öffnet sich erneut das graue Fenster, aber nichts passiert? Nicht ganz! Wechsle mit einem Klick in deiner Taskleiste zurück zum Godot Editor, während das Programm noch läuft (oder drücke die Tastenkombination ++alt+tab++). Du solltet nun im `Debugging`-Bereich unterhalb des Skripteditors das Ausgabefenster (`Output`) sehen. Darin stehen ein paar Zeilen zur Godot Engine, der OpenGL Version und deiner Grafikkarte. Und darunter solltest du nun die Zeile "Hello World" entdecken!

![Debuggingbereich mit Hello World]()

Du hast mit `print` deinen ersten GDScript-Befehl kennengelernt! Dieser schreibt alles was du willst in die Konsolenausgabe, welche du während des Testens deines Spieles beobachten kannst. Das hilft beim Finden von Fehlern oder einfach nur, um zu verstehen, wie etwas funktioniert. Sowas nennt man dann _print-Debugging_.