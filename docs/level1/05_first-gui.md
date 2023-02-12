# Erste GUI

Wann hast du das letzte Mal ein Spiel ohne Menü gesehen? Eben! Wir brauchen auch eines. Um solche sogenannten Benutzeroberflächen - oder englisch Graphical User Interface (GUI) - zu bauen, benötigt man die Control-Nodes.

Davon gibt es sehr viele. Für das Anzeigen von Text gibt es z.B. das Label. Wenn du eine Texteingabe brauchst, kannst du TextEdit verwenden. Oftmals braucht man aber auch einen Knopf zum Drücken, also etwas das auf einen Klick (oder eine Toucheingabe) reagiert - dies sind die Buttons.

Label hinzufügen

Button hinzufügen

Play -> Text wird angezeigt, Button kann geklickt werden -> Aber nichts passiert

---

Erweitert >>>...

Wie kann man Godot sagen, dass bei einem Klick auf einen Button etwas passieren soll?

Ein Klick ist ein sogenanntes Event (englisch Ereignis). Wenn dieses auftritt, können wir dem Node sagen, dass es anderen Nodes Bescheid geben soll. Das Node sendet dann ein Signal aus, dass alle empfangen können, die darauf lauschen. Man könnte auch sagen, es ruft: "Hey ihr da draußen - ich wurde geklickt!"

- Signal

print("Button wurde geklickt!")