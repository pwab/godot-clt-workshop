# Spickzettel

Die wenigsten kennen alle Sprachstrukturen und Funktionen von GDScript auswendig. Viel mehr baut man sich durch stetige Wiederholung seinen "Programmiersprachwortschatz" nach und nach auf. In der Zwischenzeit machen sich Spickzettel (englisch Cheatsheet) ganz gut - so wie in der Schule. (Das Wort "Cheat" heißt übersetzt so viel wie Betrug/Schwindel und das kommt auch [an anderer Stelle in Spielen](https://de.wikipedia.org/wiki/Cheat_(Computerspiel)) vor.)

!!! tip "Cheatsheet"
    Erstelle dir selbst einen Spickzettel für die aus deiner Sicht wichtigsten Codestrukturen und Funktionen. Diese kannst du auf ein Blatt Papier schreiben, welches du bei jedem Projekt bereitlegst, damit du schnell mal einen Befehl oder ähnliches nachschauen kannst.

## Kommentare

```gdscript
# Kommentar
```

## Variablen

```gdscript
var zahl = 5
var zeichenkette = "Hello"
var feld = [1, 2, 3]
var woerterbuch = {"key": "value", 2: 3}
var vektor2d = Vector2(1, 2)
var vektor3d = Vector3(1, 2, 3)
const KONSTANTE = 3.14
enum Kategorie {EINS, ZWEI, DREI}
```

## Annotationen

```gdscript
@onready
@export
@export_range(0, 100, 1, "or_greater", "or_lesser")
@export_group("My Properties")
```

## Funktionen

```gdscript
# Funktionsdeklaration
func summenfunktion(wert1, wert2):
    return wert1 + wert2

# Funktionsaufruf
var ergebnis = summenfunktion(1,2)
```

## Strukturen

```gdscript
if a > b:
    ...
elif a < b:
    ...
else:
    ...

match s:
    "A":
        ...
    "B":
        ...
    "C"":
        ...
```

## Schleifen

```gdscript
while a > b:
    ...

for buchstabe in ["A", "B", "C"]:
    ... # A, B, C

for i in range(5):
    ... # 0, 1, 2, 3, 4

for i in range(1, 6):
    ... # 1, 2, 3, 4, 5

for i in range(2, 12, 2):
    ... # 2, 4, 6, 8, 10
```

## Operatoren

```gdscript
+ - * / %
< > == != >= <=
!irgendwas
not irgendwas
etwas and noch_etwas 
etwas or etwas_anderes
is
in
as
```

## Typen

```gdscript
null
bool
int
float
String
Vector2
Vector3
Array
Dictionary
Color
NodePath
```

## Signale

```gdscript
# Im Skript dings.gd
signal getroffen(womit, wie_doll)

# In einer Szene mit einem Dings mit dem Namen Dingsdabums 
func _ready():
    var dingsdabums = get_node('Dingsdabums')
    dingsdabums.connect("getroffen", self, "_wenn_dings_getroffen")

func _wenn_dings_getroffen(womit, wie_doll):
    print("Wer war das: ", womit)
    print("Wie sehr tut es weh: ", wie_doll)
```

## Allgemein

```gdscript
pass
print
```

## Szenenbaum

```gdscript
get_tree().paused = true
get_tree().reload_current_scene()
get_tree().change_scene_to_file("res://levels/level2.tscn")
```

## Nodes/Szenen

```gdscript
preload
load
get_tree().get_root()
get_node("Szene/Dingsdabums")
$Dingsdabums
self

var Dings = load("res://dings.tscn")
var dingsdabums = Dings.instantiate()
get_parent().add_child(dingsdabums)
```

## Mainloop/Notifications

```gdscript
_init()
_enter_tree()
_ready()
_exit_tree()

_process(delta)
_physics_process(delta)

_input(event)
_unhandled_input(event)

_draw()
```

## Spezialzeug

```gdscript
@tool
```

## Weitere Hilfen

### Themen-Cheatsheets

- [Tweening Cheatsheet](https://i.redd.it/zdzhci8octp41.png)
- [Stretch Mode](https://i.redd.it/xlyb3wy3ozn61.png)

### Zum schnellen Nachschlagen

- [Offizielle Dokumentation - GDScript Basics](https://docs.godotengine.org/en/stable/tutorials/scripting/gdscript/gdscript_basics.html)
- [GDScript.com - Tutorials](https://gdscript.com/tutorials/)
- [GDScript.com - Solutions](https://gdscript.com/solutions/)
- [kidscancode.org - Godot Recipes](https://kidscancode.org/godot_recipes/4.x/)