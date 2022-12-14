# AMAZING MAZE
### Projektseite

von Cosima und Friederike, 12bc

## Inhaltsverzeichnis
[Projektvorstellung](https://github.com/cosima-friederike/Projektseite-AMAZING-MAZE/blob/main/README.md#projektvorstellung)

[Programm](https://github.com/cosima-friederike/Projektseite-AMAZING-MAZE/blob/main/README.md#programm)

[Aufbau und Code](https://github.com/cosima-friederike/Projektseite-AMAZING-MAZE/blob/main/README.md#aufbau-und-code)

[Arbeitstagebuch](https://github.com/cosima-friederike/informatik-c-f#informatik-projekt-cosima--friederike)

## Projektvorstellung
AMAZING MAZE ist ein 2D-Spiel, dessen Grundaufbau aus einem Labyrinth besteht und das Spielkonzept somit ist, dieses Labyrinth zu passieren und den Weg raus zu finden. Der Spieler übernimmt hierfür die Kontrolle des Player 1, der im Spiel durch einen roten Punkt dargestellt ist. 
Die Schwierigkeit des Spiels befindet sich dabei, dass der Player 1 die Wände des Labyrinths nicht berühren darf, da er sonst automatisch zurück zum Startpunkt des Spiels gelangt, welches in der Mitte des Labyrinths liegt, und dort neu starten muss. Außerdem gibt es für jedes Level nur einen richtigen Weg, um dem Labyrinth zu entkommen, alle anderen scheinbaren Wege enden in Sackgassen. Allerdings weiß der Spieler zunächst nicht, wo das Ziel und welches der richtige Weg ist, da das Spielfeld von einer Blende abgedeckt wird und lediglich der Player 1 und seine unmittelbare Umgebung zu sehen sind.
Schafft es der Spieler nun seinen Player 1 ganz durch das Labyrinth zu führen, ohne die Wände zu berühren, so erreicht er das Ziel und wird erneut zur Levelauswahl weitergeleitet. 
Insgesamt besteht das Spiel aus drei Levels, die durch zunehmende Schwierigkeitsgrade voneinander ausgemacht werden können, wie zum Beispiel durch breiterer oder schmalere Wege und mehr oder weniger Verzweigungen. 
## Programm
Wir haben uns für das Entwickeln unseres Spieles für das Programm Snap! entschieden. Dies ist gut für Anfänger, wie uns, geeignet, da es durch eine einfache Blockstruktur aufgebaut ist. Man entwickelt nicht selber einen Code, sondern arbeitet mit dem vorgegebenen Quellcode, welcher sich in den Blöcken befindet. Somit werden keine besonderen Vorkentnisse benötigt. Zudem ist das Programm durch die Blockstruktur sehr übersichtlich und problemlos den eigenen Ideen anzupassen. Daher können Fehler oder ungewünschte Programmierungen einfach vermieden und schnell behoben werden.
## Aufbau und Code
Für AMAZING MAZE haben wir sieben  verschiedene Sprites erstellt: Player 1, Labyrinth, Finish, Blende, Start, Screen und das Level. Da es drei Spiellevels gibt, haben wir für das zweite und dritte Level jeweils ein neues Labyrinth, Finish und natürlich die Levelauswahl programmiert. Die Sprites, die nur für ein spezifisches Level benötigt werden, sind mit der Funktion "hide" dabei so programmiert, dass sie von der Spielfläche scheinbar verschwinden und die Funktionen ausgestellt sind, wenn ein anderes Level gewählt wurde. 

![Screenshot (13)](https://user-images.githubusercontent.com/111414772/207529351-7198e1c0-3428-4c94-a283-51b433e2d9de.png)
Auf dem Bild sehen Sie die Sprites Labyrinth, Player 1 und Finish. Die Blende, die eigentlich bei jedem Level erscheint, haben wir für das Foto ausgestellt, um das Labyrinth und die anderen Sprites besser zeigen zu können. Zusätzlich haben wir ein Foto für den Hintergrund des Labyrinths eingefügt, um die Spieloptik interessanter und das Spielen schwieriger zu gestalten.
#### Player 1
Dieser Sprite stellt die Spielfigur des Spielers dar und wird mit Hilfe der vier Pfeiltasten gesteuert. Zu Beginn jedes Spiels, befindet sich der Sprite im Center des Labyrinths. Damit der Player 1 automatisch zum Startpunkt gelangt, wenn dieser die Labyrinthwände berührt, haben wir einen broadcast mit dem Befehl center erstellt. Diese Funktion gibt es für jedes Level einzeln. Zusätzlich erscheint noch eine Sprechblase mit dem Ausruf "aaahh!!" beim Berühren der Wände.

![Unbenannt](https://user-images.githubusercontent.com/111414772/207534250-85f4ca3c-bd1e-4b51-a7f8-0c483cef9315.png)
#### Labyrinth
Für die drei Sprites Labyrinth 1, 2 und 3 haben wir jeweils nur ein Kostüm erstellt, Funktionen und Befehle gibt es keine.
#### Finish
Der Sprite Finish stellt das Ziel des Spiels dar, das der Player 1 erreichen muss. Für jedes Level mit eigenem Labyrinth gibt es auch ein sperates Ziel. Die Funktionen sind allerdings grundsätzlich übereinstimmend und nur auf das jeweilige Level angepasst. Sobald der Spieler das Ziel erreicht, wird der Befehl finish ausgeführt, das heißt, es werden alle Sprites samt ihrer Funktionen versteckt, die Levelauswahl und der Screen ausgenommen.

![Finish](https://user-images.githubusercontent.com/111414772/207535843-2e8d638b-5697-4a52-86d7-a775c5c93c1d.png)
#### Blende
Die Blende ist durch die Funktion "point towards Player 1" und die gleichen Bewegungsbefehle durch die Pfeiltasten, wie der Player 1, so programmiert, dass die diesem folgt, damit der Spieler sowie seine unmittelbare Umgebung immer sichtbar sind. Die hauptsächliche Aufgabe der Blende ist es, den Schwierigkeitsgrad des Spiels zu erhöhen, damit der Spieler nicht das ganze Labyrinth und das Ziel sieht. Wie beim Player 1 gibt es den Befehl, dass sich die Blende zu Beginn des Spieles im Center befindet.

![Blende](https://user-images.githubusercontent.com/111414772/207539407-814cd143-6cb2-4306-9018-9e145e0d5c95.png)
#### Start
Dieser Sprite stellt den Spielstart dar. Wird auf den Startbutton geklickt, gelangt der Spieler zur Levelauswahl, indem die drei Sprites der Levels erscheinen und der Startsprite versteckt wird.

![Start](https://user-images.githubusercontent.com/111414772/207540084-52b0c784-2e3b-4339-8a70-e33d45c42f76.png)
#### Screen
Dies ist der Hintergrund der Sprites Start und Level und wird bei der Auswahl eines Levels versteckt.

![Screen](https://user-images.githubusercontent.com/111414772/207540457-46f179e5-ff6b-4da2-abdc-e902e2b130ac.png)
#### Levelauswahl
Die Levelauswahl besteht aus den drei Sprites Level 1, 2 und 3. Diese werden gezeigt, wenn der Start aktiviert wird. Dann kann sich der Spieler für ein Level entscheiden, indem er mit dem Mauscursor darauf klickt. Daraufhin werden alle, zu dem Level gehörenden Sprites, gezeigt, die anderen werden versteckt. 

![Levels](https://user-images.githubusercontent.com/111414772/207542083-d20aec4a-5cf6-47b0-ac69-7508af14f603.png)
