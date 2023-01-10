# Hello World

## Assets

Am besten lädst du dir jetzt [dieses Asset-Pack](../assets/assets.zip) herunter und entpackst es in einen beliebigen Ordner. Assets sind Materialien, welche in einem Spiel eingesetzt werden. Dazu zählen Bilder, Soundeffekte oder auch Schriftarten. Dieses Asset-Pack enthält mehrere Dateien, welche wir im Workshop verwenden werden und welche du anschließend für eigene Spiele benutzen kannst. Alle Materialien stehen unter der offenen CC0-Lizenz (nennt man auch Public Domain) und dürfen deshalb frei und kostenlos für alle Projekte verwendet werden.

## Dein erstes Projekt

Jetzt wird es Zeit für das erste eigene Projekt und die erste Zeile Code! Schließe dazu die `2D Platformer` Demo oben links im Hauptmenü mit einem Klick auf `Projekt` und dann `Zur Projektverwaltung zurückkehren`. Godot wird dich fragen, ob du das aktuelle Projekt wirklich schließen möchtest. Das kannst du mit Ja bestätigen - eventuell geänderte Szenen kannst du dabei gern speichern.

!!! warning "Baustelle"
    Sorry, ab hier fehlt noch einiges. Ich arbeite daran ⛏

In der Projektverwaltung

- Neues Projekt
- Titel
- Ordner
- Bearbeiten und Erstellen

Leeres Projekt ist wie ein leeres Blatt Papier

![]()

## Deine erste Zeile Code

Nodes hinzufügen

Node2D

Skript -> GDScript

Code Vorlage (Template):

```gdscript
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

Dort unter `func _ready():` das `pass` entfernen und dann mit einem Tab eingerückt `print("Hello World")` eingeben:

```gdscript
func _ready():
    print("Hello World")
```

## Deine erste GUI

- Label
- Button
- Signal

## Dein erstes Bild

- Sprite mit Godot Icon beim Klick auf den Button

## Deine erste Animation

- Drehen des Sprites beim Klick auf den Button

## Dein erster Sound

- "Click" beim Klick auf den Button

## Deine erste Steuerung

- Tastatur Pfeil + WASD
- Bewegung des Sprites

!!! success "Level 1: Complete"

    Du hast es geschafft, auf zu Level 2!