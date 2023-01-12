# Erster Code

Nodes hinzufügen

Node2D

Skript -> GDScript

Code Vorlage (Template):

```gdscript title="Template" linenums="1" hl_lines="9 10"
extends Node2D

# Declare member variables here. Examples:
# var a = 2
# var b = "text"


# Called when the node enters the scene tree for the first time.
func _ready():
	pass # Replace with function body.


# Called every frame. 'delta' is the elapsed time since the previous frame.
#func _process(delta):
#	pass
```

Dort in Zeile 10 unter `#!gdscript func _ready():` das `#!gdscript pass` entfernen und dann mit einem ++tab++ eingerückt `#!gdscript print("Hello World")` eingeben:

```gdscript linenums="9"
func _ready():
    print("Hello World")
```
