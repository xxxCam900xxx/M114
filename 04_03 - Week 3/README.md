# Title

### Inhaltsverzeichnis
- [Title](#title)
    - [Inhaltsverzeichnis](#inhaltsverzeichnis)
- [Theorie](#theorie)
    - [VLC](#vlc)
    - [RLC](#rlc)
    - [RLE](#rle)
- [Aufgabe 1](#aufgabe-1)
- [Aufgabe 2](#aufgabe-2)
- [Aufgabe 3](#aufgabe-3)
- [Aufgabe 4](#aufgabe-4)

---------------------------------------
# Theorie
### VLC

![VLC](/04_03%20-%20Week%203/Content/VLC.jpg)

### RLC

![RLC](/04_03%20-%20Week%203/Content/RLE.png)

### RLE
Run-length encoding (RLE) ist ein sehr einfaches Datenkompressionsverfahren, welches bei Folgen gleicher Zeichen deren Häufigkeit angibt. Es erzeugt nur gute Ergebnisse, wenn lange Folgen gleicher Daten vorliegen, was häufig bei Graphiken der Fall sein dürfte. Deshalb verwendet es z.B. Microsoft im .bmp-Format. Andere Einsatzmöglichkeiten sind Textdateien, bei denen Leerzeichen zum Formatieren verwendet wurden.

RLE ist ein verlustfreies Verfahren mit geringer Kompressionsrate. Es ist aber einfach zu verstehen, zu implementieren und auszuführen.

# Aufgabe 1
**Huffman-Algorithmus**: Wir beschäftigen uns hier mit sogenannten Baumstrukturen. 
Kennen sie noch andere Gebiete in der IT, wo Baumstrukturen zur Anwendung 
kommen? Beim Huffman handelt es sich sogar um eine spezielle Baumstruktur, 
nämlich einem sogenannten binären Baum. Was unterscheidet einen binären Baum 
von einem nicht binären Baum?

[Huffman-Algorithmus](/Huffmann/README.md)

# Aufgabe 2
**Huffman-Algorithmus**: In dieser Aufgabe arbeiten sie zu zweit: Jeder denkt sich ein 
Wort mit ca. 15 Buchstaben aus und erstellt dazu den Huffman-Code inkl. 
Codetabelle und das entsprechend komprimierte Wort in Binärdarstellung. Tauschen 
sie ihre Codes und Codetabellen gegenseitig aus und vergewissern sie sich, dass ihr 
Partner ihr gewähltes Wort richtig dekomprimieren kann. Sie haben die Aufgabe dann 
vollständig gelöst, wenn sie einen korrekten binären Baum vorweisen können, die 
Codes herausgelesen und tabellarisch notiert haben und das komprimierte Wort in
Huffman-Binärcode nicht fehlt.

[Huffman-Algorithmus](/Huffmann/README.md)

# Aufgabe 3
**RLC**: Wie könnte die Komprimierung ausschauen, wenn es sich anstatt um ein 
Schwarz/Weissbild, um ein Farbbild handelt?
![RLC](/04_03%20-%20Week%203/Content/Aufgabe3-RLC.png)
Benachbarte Pixel mit identischer Farbe werden ja bei RLC bekanntlich nicht einzeln 
genannt, sondern zu einer Anzahl zusammengefasst wie z.B. **11xGrün, 6xBlau, 
3xWeiss etc. oder in binärer Schreibweise 1011Grün, 0110Blau, 0011Weiss.** Welche 
Bitbreite (1011Grün ergäbe 4 Bit) wäre bei einem quadratischen Bild mit 20 Pixel 
Kantenlänge sinnvoll? Was wäre, wenn dieses Bild nur aus einer Farbe besteht?

In einem quadratischen Bild mit 20 Pixel Kantenlänge gibt es insgesamt 400 Pixel. Wenn das gesamte Bild aus einer einzigen Farbe besteht, hätten wir eine maximale Anzahl von aufeinanderfolgenden Pixeln mit derselben Farbe von 400.

Um diese Anzahl binär darzustellen, benötigen wir 9 Bits (2^9 = 512 > 400, aber 2^8 = 256 < 400). Daher wäre eine Bitbreite von 9 Bits sinnvoll, um die RLC-Codierung zu verwenden, wenn das Bild nur aus einer Farbe besteht.

# Aufgabe 4
**RLC**: Sie erhalten diesen RL-Code:
```
010100011110010010010010010010010010010110010110010010010010010010010010001
```
Folgendes ist ihnen dazu bekannt: Es handelt sich um eine quadratische Schwarz-Weiss-Rastergrafik mit einer Kantenlänge von 8 Pixel. Es wird links oben mit der 
Farbe Weiss begonnen. Eine Farbe kann sich nicht mehr als siebenmal wiederholen. 
Zeichnen sie die Grafik auf. Was stellt sie dar?
