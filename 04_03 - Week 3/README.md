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
- [Aufgabe 5](#aufgabe-5)
- [Aufgabe 6](#aufgabe-6)
    - [Rotiert](#rotiert)
    - [Alphabethisch](#alphabethisch)

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

# Aufgabe 5
LZW-Verfahren
a. Erstellen sie die LZW-Codierung für das Wort «ANANAS» und überprüfen sie 
mit der Dekodierung ihr Resultat. 

| Schritt | Zeichenkette | Gefunden | Gespeichert | Temp Wörterbuch |
| --- | --- | --- | --- | --- |
| 1. | **A**NANAS | A | **A** | AN -> 256 |
| 2. | **N**ANAS | N | **N** | NA -> 257 |
| 3. | **A**NAS | AN | **256** | ANA -> 258 |
| 4. | **N**AS | NA | **257** | NAS -> 259 |

b. Versuchen sie den erhaltenen LZW-Code «ERDBE<256>KL<260>» zu 
dekomprimieren.
| Schritt | Zeichenkette | Gefunden | Gespeichert | Temp Wörterbuch |
| --- | --- | --- | --- | --- |
| 1. | **E**RDBE<256>KL<260> | E | **E** | - |
| 2. | E**R**DBE<256>KL<260> | R | **R** | ER -> 256 |
| 3. | ER**D**BE<256>KL<260> | D | **D** | RD -> 257 |
| 4. | ERD**B**E<256>KL<260> | B | **B** | DB -> 258 |
| 5. | ERDB**E**<256>KL<260> | E | **E** | BE -> 259 |
| 6. | ERDBE **<256>** KL<260> | 256 | **256** | EE -> 260 |
| 7. | ERDBE<256>**K**L<260> | K | **K** | RL -> 261 |
| 8. | ERDBE<256>K**L**<260> | L | **L** | KL -> 262 |
| 9. | ERDBE<256>KL **<260>** | 260 | **260** | LE -> 263 |

Lösung : **ERDBEERKLEE**

# Aufgabe 6
**BWT** (Burrows-Wheeler-Transformation):
a. Erstellen sie die BWT-Transformation für das Wort ANANAS und überprüfen 
sie mit der Rücktransformation ihr Resultat.

### Rotiert
| Zeile | Wort |
| --- | --- |
| 1. | **A**NANAS |
| 2. | S**A**NANA |
| 3. | AS**A**NAN |
| 4. | NAS**A**NA |
| 5. | ANAS**A**N |
| 6. | NANAS**A** |

### Alphabethisch
| Zeile | Wort |
| --- | --- |
| 1. | **A**NANAS |
| 2. | 

b. Sie erhalten den Code IICRTGH6 in der Burrows-Wheeler-Transformation. 
Welches Wort verbirgt sich dahinter?