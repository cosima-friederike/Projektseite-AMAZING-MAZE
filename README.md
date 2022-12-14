# Projektseite

von Cosima und Friederike, 12bc

## Inhaltsverzeichnis
[Projektvorstellung](https://github.com/cosima-friederike/Projektseite/blob/main/README.md#projektvorstellung-1)

[Programm](https://github.com/cosima-friederike/Projektseite/blob/main/README.md#programm)

[Aufbau](https://github.com/cosima-friederike/Projektseite/blob/main/README.md#aufbau)

[Arbeitstagebuch](https://github.com/cosima-friederike/informatik-c-f#informatik-projekt-cosima--friederike)

## Projektvorstellung
"AMAZING MAZE" ist ein 2D-Spiel, dessen Grundaufbau aus einem Labyrinth besteht und das Spielkonzept somit ist, dieses Labyrinth zu passieren und den Weg raus zu finden. Der Spieler übernimmt hierfür die Kontrolle des "Player 1", der im Spiel durch einen roten Punkt dargestellt ist. 
Die Schwierigkeit des Spiels befindet sich dabei, dass der "Player 1" die Wände des Labyrinths nicht berühren darf, da er sonst automatisch zurück zum Startpunkt des Spiels gelangt, welches in der Mitte des Labyrinths liegt, und dort neu starten muss. Außerdem gibt es für jedes Level nur einen richtigen Weg, um dem Labyrinth zu entkommen, alle anderen scheinbaren Wege enden in Sackgassen. Allerdings weiß der Spieler zunächst nicht, wo das Ziel und welches der richtige Weg ist, da das Spielfeld von einer Blende abgedeckt wird und lediglich der "Player 1" und seine unmittelbare Umgebung zu sehen ist.
Schafft es der Spieler nun seinen "Player 1" ganz durch das Labyrinth zu führen, ohne die Wände zu berühren, so erreicht er das Ziel und wird erneut zur Levelauswahl weitergeleitet. 
Insgesamt besteht das Spiel aus drei Levels, die durch zunehmende Schwierigkeitsgrade voneinander ausgemacht werden können, wie zum Beispiel durch breiterer oder schmalere Wege und mehr oder weniger Verzweigungen. 
## Programm
Wir haben uns für das Entwickeln unseres Spieles für das Programm Snap! entschieden. Dies ist gut für Anfänger, wie uns, geeignet, da es durch eine einfache Blockstruktur aufgebaut ist. Man entwickelt nicht selber einen Code, sondern arbeitet mit dem vorgegebenen Quellcode, welcher sich in den Blöcken befindet. Somit werden keine besonderen Vorkentnisse benötigt. Zudem ist das Programm durch die Blockstruktur sehr übersichtlich und problemlos den eigenen Ideen anzupassen. Daher können Fehler oder ungewünschte Programmierungen einfach vermieden und schnell behoben werden.
## Aufbau
### Sprites
Für AMAZING MAZE haben wir sieben  verschiedene Sprites erstellt: Player 1, Labyrinth, Finish, Blende, Start, Screen und das Level. Da es drei Spiellevels gibt, haben wir für das zweite und dritte Level jeweils ein neues Labyrinth, Finish und natürlich die Levelauswahl programmiert. Die Sprites, die nur für ein spezifisches Level benötigt werden, sind mit der Funktion "hide" dabei so programmiert, dass sie von der Spielfläche scheinbar verschwinden und die Funktionen ausgestellt sind, wenn ein anderes Level gewählt wurde. 

![Screenshot (13)](https://user-images.githubusercontent.com/111414772/207529351-7198e1c0-3428-4c94-a283-51b433e2d9de.png)
Auf dem Bild sehen Sie die Sprites Labyrinth, Player 1 und Finish. Die Blende, die eigentlich bei jedem Level erscheint, haben wir für das Foto ausgestellt, um das Labyrinth und die anderen Sprites besser zeigen zu können.
#### Player 1
Dieser Sprite stellt die Spielfigur des Spielers dar und wird mit Hilfe der vier Pfeiltasten gesteuert. Zu Beginn jedes Spiels, befindet sich der Sprite im Center des Labyrinths. Damit der Player 1 automatisch zum Startpunkt gelangt, wenn dieser die Labyrinthwände berührt, haben wir einen broadcast mit dem Befehl center erstellt. Diese Funktion gibt es für jeden Level einzeln.

![Unbenannt](https://user-images.githubusercontent.com/111414772/207534250-85f4ca3c-bd1e-4b51-a7f8-0c483cef9315.png)
#### Labyrinth
Für die drei Sprites Labyrinth 1, 2 und 3 haben wir jeweils nur ein Kostüm erstellt, Funktionen und Befehle gibt es keine.
#### Finish
Der Sprite Finish stellt das Ziel des Spiels dar, das der Player 1 erreichen muss. Für jedes Level mit eigenem Labyrinth gibt es auch ein sperates Ziel. Die Funktionen sind allerdings grundsätzlich übereinstimmend und nur auf das jeweilige Level angepasst. Sobald der Spieler das Ziel erreicht, wird der Befehl finish ausgeführt, das heißt, es werden alle Sprites samt ihrer Funktionen versteckt, die Levelauswahl und der Screen ausgenommen.

![Finish](https://user-images.githubusercontent.com/111414772/207535843-2e8d638b-5697-4a52-86d7-a775c5c93c1d.png)
#### Blende
#### Start
#### Screen
#### Levelauswahl
