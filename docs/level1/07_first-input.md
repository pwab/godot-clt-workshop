# Erste Steuerung

Eingabe der Pfeiltasten soll Bild bewegen

Koordinatensystem xy

Position des Bildes laut Nodeeigenschaften

Nach links/rechts verschieben --> x-Wert ändert sich
Nach oben/unten verschieben --> y-Wert ändert sich

Zurück zum Code

func _input(event):
    if event.is_action("ui_right"):
        image.position.x += 1
    elif event.is_action("ui_left"):
        image.position.x -= 1

etc.

!!! success "Level 1: Complete"

    Du hast es geschafft, auf zu Level 2!