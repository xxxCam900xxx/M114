# A_DATEN_CODIEREN_NUM_ANNE

### Inhaltsverzeichnis
- [X] [Aufgabe 1 - DEZ / HEX / BIN](#aufgabe-1---dez--hex--bin)
- [X] [Aufgabe 2 - DEZ to BIN](#aufgabe-2---dez-to-bin)
- [X] [Aufgabe 3 - BIN to DEZ](#aufgabe-3---bin-to-dez)
- [X] [Aufgabe 4 - BIN to HEX](#aufgabe-4---bin-to-hex)
- [X] [Aufgabe 5 - BIN + BIN](#aufgabe-5---bin--bin)
- [X] [Aufgabe 6 - Zusätzliches Umwandeln](#aufgabe-6---zusätzliches-umwandeln)
- [X] [Aufgabe 7 - Linux 751](#aufgabe-7---linux-751)
- [X] [Aufgabe 8 - Matterhorn-Express](#aufgabe-8---matterhorn-express)
- [X] [Aufgabe 9 - Arbeitspeicher](#aufgabe-9---arbeitspeicher)
- [ ] [Aufgabe 10 - Taktsignal](#aufgabe-10---taktsignal)
- [ ] [Aufgabe 11 - Zusatz Aufgaben](#aufgabe-11---zusatz-aufgaben)
- [ ] [Aufgabe 12 - Fliesskommazahlen](#aufgabe-12---fliesskommazahlen)
- [X] [Aufgabe 13 - AND / OR / NOT / EXOR](#aufgabe-13---and--or--not--exor)
- [X] [Aufgabe 14 - Modulo Funktion](#aufgabe-14---modulo-funktion)
- [X] [Reflexion](#reflexion)

# Aufgabe 1 - DEZ / HEX / BIN
Erstellen sie eine leere Tabelle mit 6 Kolonnen und 16 Zeilen. Füllen sie diese wie 
folgt aus:
1. Kolonne: Dezimalzahlen von 0 bis 15
2. Kolonne: Hexadezimalzahlen von 0 bis F
3. Kolonne, 4. Kolonne, 5. Kolonne und 6. Kolonne die entsprechenden Binärzahlen
Studieren sie nun ihre fertig ausgefüllte Tabelle, insbesondere die Kolonnen mit den 
Binärwerten. Was stellen sie fest

| DEZ | HEX | BIN | 8 | 4 | 2 | 1 |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| 0 | 0 |  | 0 | 0 | 0 | 0 |
| 1 | 1 |  | 0 | 0 | 0 | 1 |
| 2 | 2 |  | 0 | 0 | 1 | 0 |
| 3 | 3 |  | 0 | 0 | 1 | 1 |
| 4 | 4 |  | 0 | 1 | 0 | 0 |
| 5 | 5 |  | 0 | 1 | 0 | 1 |
| 6 | 6 |  | 0 | 1 | 1 | 0 |
| 7 | 7 |  | 0 | 1 | 1 | 1 |
| 8 | 8 |  | 1 | 0 | 0 | 0 |
| 9 | 9 |  | 1 | 0 | 0 | 1 |
| 10 | A |  | 1 | 0 | 1 | 0 |
| 11 | B |  | 1 | 0 | 1 | 1 |
| 12 | C |  | 1 | 1 | 0 | 0 |
| 13 | D |  | 1 | 1 | 0 | 1 |
| 14 | E |  | 1 | 1 | 1 | 0 |
| 15 | F |  | 1 | 1 | 1 | 1 |

# Aufgabe 2 - DEZ to BIN
Wandeln sie die folgende Dezimalzahl ohne Taschenrechner in die entsprechende 
Binärzahl um: **911**

| 2048 | 1024 | 512 | 256 | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |  
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| 0 | 0 | 1 | 1 | 1 | 0 | 0 | 0 | 1 | 1 | 1 | 1 |

**oder**

- 911 / 2 = 455 | R-1
- 455 / 2 = 227 | R-1
- 227 / 2 = 113 | R-1
- 113 / 2 = 56  | R-1
- 56  / 2 = 28  | R-0
- 28  / 2 = 14  | R-0
- 14  / 2 = 7   | R-0
- 7   / 2 = 3   | R-1
- 3   / 2 = 1   | R-1
- 1   / 2 = 0   | R-1
- **1 1 1 1 0 0 0 1 1 1**

# Aufgabe 3 - BIN to DEZ
Wandeln sie die folgende Binärzahl ohne Taschenrechner in die entsprechende 
Dezimalzahl um: 1011'0110

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| 1 | 0 | 1 | 1 | 0 | 1 | 1 | 0 |

128 + 32 + 16 + 4 + 2 = **182**

# Aufgabe 4 - BIN to HEX
Wandeln sie die folgende Binärzahl ohne Taschenrechner in die entsprechende 
Hexadezimalzahl um: **1110'0010'1010'0101**

| 8 | 4 | 2 | 1 | | 8 | 4 | 2 | 1 | | 8 | 4 | 2 | 1 | | 8 | 4 | 2 | 1 |  
| - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - |  
| 1 | 1 | 1 | 0 | - | 0 | 0 | 1 | 0 | - | 1 | 0 | 1 | 0 | - | 0 | 1 | 0 | 1 |  
| **E** | - | - | - | - | **2** | - | - | - | - | **A** | - | - | - | - | **5** | - | - | - |  

# Aufgabe 5 - BIN + BIN
Was ergibt die Addition der beiden binären Zahlen 1101'1001 und 0111'0101?
Beachten sie, dass für das Resultat ebenfalls nur 8 Binärstellen zur Verfügung 
stehen.

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| - | - | - | - | - | - | - | - |
| 1 | 1 | 0 | 1 | 1 | 0 | 0 | 1 |

128 + 64 + 16 + 8 + 1 = **217**


| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| - | - | - | - | - | - | - | - |
| 0 | 1 | 1 | 1 | 0 | 1 | 0 | 1 |

64 + 32 + 16 + 4 + 1 = **117**

---------------

217 + 121 = **334**

- 334 / 2 = 167 | R-0
- 167 / 2 = 83  | R-1
- 83  / 2 = 41  | R-1
- 41  / 2 = 20  | R-1
- 20  / 2 = 10  | R-0
- 10  / 2 = 5   | R-0
- 5   / 2 = 2   | R-1
- 2   / 2 = 1   | R-0
- ----------------------
- 1   / 2 = 0   | R-1
- ----------------------
- **0 1 0 0 1 1 1 0**

oder

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| - | - | - | - | - | - | - | - |
| 0 | 1 | 1 | 1 | 0 | 1 | 0 | 1 |
| 1 | 1 | 0 | 1 | 1 | 0 | 0 | 1 |
| - | - | - | - | - | - | - | - |
| 1 | 1 | 1 | - | - | - | 1 | - |
| - | - | - | - | - | - | - | - |
| 0 | 1 | 0 | 0 | 1 | 1 | 1 | 0 |

# Aufgabe 6 - Zusätzliches Umwandeln
Was könnten die beiden folgenden binären Wert für eine Bedeutung haben?
(Tipp: a. ins Dezimalsystem umrechnen, b. ins Hexadezimalsystem umrechnen)
- a. 1100’0000.1010’1000.0100’1100.1101’0011
- b. 1011’1110-1000’0011-1000’0101-1101’0101-1110’0100-1111’1110

### a - DEZ

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| - | - | - | - | - | - | - | - |
| 1 | 1 | 0 | 0 | 0 | 0 | 0 | 0 |

128 + 64 = **192**

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| - | - | - | - | - | - | - | - |
| 1 | 0 | 1 | 0 | 1 | 0 | 0 | 0 |

128 + 32 + 8 = **168**

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| - | - | - | - | - | - | - | - |
| 0 | 1 | 0 | 0 | 1 | 1 | 0 | 0 |

64 + 8 + 4 = **76**

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| - | - | - | - | - | - | - | - |
| 1 | 1 | 0 | 1 | 0 | 0 | 1 | 1 |

128 + 64 + 16 + 2 + 1 = **211**

### Ergibt = 192.168.76.211

### b - HEX

1011'1110 -> BE
1000'0011 -> 83
1000'0101 -> 85
1101'0101 -> D5
1110'0100 -> E4
1111'1110 -> FE

# Aufgabe 7 - Linux 751
Für Linux-Fans: Was könnte die folgende in einem Bash-Script entdeckte Zeile für 
eine Bedeutung haben? chmod 751 CreateWeeklyReport

chmod 751 CreateWeeklyReport

hat die Bedeutung, dass die Zugriffsrechte für die Datei "CreateWeeklyReport" geändert werden. "chmod" ist ein Befehl in Linux/Unix-Systemen, der verwendet wird, um die Zugriffsrechte von Dateien und Verzeichnissen zu ändern.

Die Zahlen "751" sind die Oktalrepräsentation der Zugriffsrechte. In diesem Fall bedeutet es:

Der Eigentümer der Datei hat Lese-, Schreib- und Ausführungsrechte (7).
Die Benutzergruppe, zu der die Datei gehört, hat Lese- und Ausführungsrechte (5).
Andere Benutzer haben nur Ausführungsrechte (1).
Zusammengefasst bedeutet dies, dass der Eigentümer volle Zugriffsrechte auf die Datei hat, die Benutzergruppe Lese- und Ausführungsrechte hat, und andere Benutzer nur die Ausführung der Datei erlaubt ist.

In diesem Fall wird die Datei "CreateWeeklyReport" wahrscheinlich so konfiguriert, dass sie vom Eigentümer bearbeitet und ausgeführt werden kann, von Mitgliedern der Benutzergruppe ausgeführt werden kann, aber nur die Ausführung für andere Benutzer erlaubt ist.

# Aufgabe 8 - Matterhorn-Express
Dimensionieren sie für den Matterhorn-Express, wo insgesamt 107 Gondeln die 
Touristen von Zermatt auf den Trockenen-Steg befördern, die Codebreite des 
Binärcodes für die Kabinenzählung?

Die nächsthöhere Potenz von 2, die größer oder gleich 107 ist, ist 128 (2^7). Das bedeutet, dass wir mindestens 7 Bits benötigen, um 107 Gondeln zu repräsentieren. 

- Die Binärdarstellung von 107 ist 1101011.
- Da wir 7 Bits benötigen, um die Kabinenzählung zu codieren, beträgt die Codebreite des Binärcodes 7.

# Aufgabe 9 - Arbeitspeicher
Sie untersuchen einen Arbeitsspeicher mit 12-Bit-Adress- bzw. 16-Bit-Datenbus.
Welche Speicherkapazität in kiB besitzt dieser? (Hinweis: 1kiB=1024B)

Speicherkapazität = 2^Adressbus * Datenbus

Speicherkapazität = 2^12 * 16 = 65536 (Bits)

**65536 / (8 * 1024) = 8 (kiB)**

# Aufgabe 10 - Taktsignal
Zwei Geräte sind mit einer seriellen Leitung und zusätzlichem Taktsignal verbunden. 
Das Taktsignal beträgt 1MHz.
- a. Wie viele Bytes können damit pro Sekunde übertragen werden?
- b. Wie viele Bytes pro Sekunde könnten übertragen werden, wenn die 
Verbindung der beiden Geräte nicht seriell, sondern 8 Bit-parallel wäre

### TO BE CONTINUE...

# Aufgabe 11 - Zusatz Aufgaben
Bei den bisherigen Aufgaben zu Binärcodes, handelte es sich immer um positive, 
numerische Werte. Bei den Programmiersprachen spricht man vom Datentyp 
"unsigned integer". Hin und wieder möchte man aber auch die negative Zahlenwelt 
miteinbeziehen, man nennt dies dann "signed integer", was mit vorzeichenbehafteter
Ganzzahl übersetzt werden kann.
(Wobei man gut beraten ist, abzuwägen, ob der Mehraufwand für negative Zahlen tatsächlich 
gerechtfertigt ist, wie folgendes Beispiel aus der Physik zeigt: Die Celsius-Temperaturskala kennt 
negative Werte, die Kelvin-Temperaturskala hingegen nicht und beide Skalen messen dieselbe 
Temperatur. Zum Beispiel entspricht der absolute Temperatur-Nullpunkt (nichts kann kälter sein, dass ist 
in diesem Fall entscheidend) -273 Grad Celsius aber eben auch 0 Grad Kelvin, Wasser schmilzt bei 0 
Grad Celsius bzw. 273 Grad Kelvin und der heutige Sommer bot angenehme 35 Grad Celsius oder eben 
308 Grad Kelvin)
Möchte man den binären Zahlenstrahl in den negativen Bereich erweitern, liegt die 
Versuchung nahe, das erste Bit (MSB) als Vorzeichen zu verwenden. Funktioniert 
leider nicht bzw. nicht in allen Fällen! Die Lösung die funktioniert, nennt man 
Zweierkomplement. Was darunter zu verstehen ist, wird im Internet unzählige Male 
erklärt.
Nun zur Aufgabe: Wir gehen von einer Verarbeitungsbreite von einem Byte aus. 
(Datenbusbreite:1Byte)
- a. Nennen sie kleinster und grösster Binärwert bzw. Dezimaläquivalent im Falle 
von unsigned bzw. Vorzeichenlos.
- b. Nennen sie kleinster und grösster Binärwert bzw. Dezimaläquivalent im Falle 
von signed bzw. Vorzeichenbehaftet.
- c. Wandeln sie die Dezimalzahl +83 in einen vorzeichenbehafteten Binärwert 
um. (signed)
- d. Wandeln sie die Dezimalzahl -83 in einen vorzeichenbehafteten Binärwert um. 
Signed mit 2er-Komplement: 
- e. Addieren sie die beiden erhaltenen Binärwerte zusammen. Es sollte 0 
ergeben!
- f. Wandeln sie die Dezimalzahl 0 in einen vorzeichenbehafteten Binärwert um. 
(signed). Hat ihre vorangegangene Addition auch diesen Binärwert ergeben?
- g. Warum können sie bei der gegebenen Datenbusbreite von 1 Byte die 
Dezimalzahl +150 nicht in einen vorzeichenbehafteten Binärwert umwandeln? 
(Ziehen sie daraus ihre Lehren für zukünftige Programmiersprachkurse: Immer den korrekten 
Datentyp in der verlangten Grösse wählen

### TO BE CONTINUE...

# Aufgabe 12 - Fliesskommazahlen
Bisher haben wir immer von ganzen Zahlen gesprochen. Oft genügt das in der realen 
Welt aber nicht. Dazu ein Beispiel: Teile ich die Ganzzahl 1 durch die Ganzzahl 3 und 
multipliziere sie darauf wieder mit der Ganzzahl 3 erhalte ich, sofern der 
Compiler/Interpreter nicht trickst, die Ganzzahl 0, was bekanntlich falsch ist. Dies weil 
das Resultat der Division nicht als 0.3333333 sondern als ganze Zahl 0 
(Nachkommastellen werden ignoriert) zwischengespeichert wird. Benötigt wird also 
ein Datentyp, der mit Fliesskommazahlen (Floating Point Numbers) klarkommt. Wie 
würden sie eine solche Fliesskommazahl definieren, und wie sie digital abspeichern? 
Machen sie dazu einen Vorschlag.

### TO BE CONTINUE...

# Aufgabe 13 - AND / OR / NOT / EXOR
Erstellen sie die Wahrheitstabellen für die folgenden Funktionen:
- a. Logisch UND/AND (mit zwei Eingangs- und einer Ausgangsvariablen)
- b. Logisch ODER/OR (mit zwei Eingangs- und einer Ausgangsvariablen)
- c. Logisch NICHT/NOT (mit einer Eingangs- und einer Ausgangsvariablen)
- d. Logisch EXOR (mit zwei Eingangs- und einer Ausgangsvariablen)

### a. Logisch UND/AND (mit zwei Eingangs- und einer Ausgangsvariablen)
In dieser Tabelle werden alle möglichen Kombinationen der Eingangsvariablen A und B aufgeführt, und die Ausgangsvariable Y gibt den entsprechenden Wert für die UND/AND-Funktion an. Das Ergebnis ist 1 (wahr), wenn beide Eingangsvariablen den Wert 1 haben, andernfalls ist es 0 (falsch).
| A | B | | Y |
| - | - | - | - |
| 0 | 0 | | 0 |
| 0 | 1 | | 0 |
| 1 | 0 | | 0 |
| 1 | 1 | | 1 |

### b. Logisch ODER/OR (mit zwei Eingangs- und einer Ausgangsvariablen)
In dieser Tabelle werden alle möglichen Kombinationen der Eingangsvariablen A und B aufgeführt, und die Ausgangsvariable Y gibt den entsprechenden Wert für die ODER/OR-Funktion an. Das Ergebnis ist 1 (wahr), wenn mindestens eine der beiden Eingangsvariablen den Wert 1 hat, andernfalls ist es 0 (falsch).
| A | B | | Y |
| - | - | - | - |
| 0 | 0 | | 0 |
| 0 | 1 | | 1 |
| 1 | 0 | | 1 |
| 1 | 1 | | 1 |

### c. Logisch NICHT/NOT
In dieser Tabelle werden alle möglichen Werte der Eingangsvariable A aufgeführt, und die Ausgangsvariable Y gibt den entsprechenden Wert für die NOT-Funktion an. Das Ergebnis ist 1 (wahr), wenn die Eingangsvariable den Wert 0 hat, und 0 (falsch), wenn die Eingangsvariable den Wert 1 hat. Die NOT-Funktion invertiert den Wert der Eingangsvariable.
| A | | Y |
| - | - | - |
| 0 | | 1 |
| 1 | | 0 |

### d. Logisch EXOR
In dieser Tabelle werden alle möglichen Kombinationen der Eingangsvariablen A und B aufgeführt, und die Ausgangsvariable Y gibt den entsprechenden Wert für die XOR-Funktion an. Das Ergebnis ist 1 (wahr), wenn genau eine der beiden Eingangsvariablen den Wert 1 hat, andernfalls ist es 0 (falsch).

| A | B | | Y |
| - | - | - | - |
| 0 | 0 | | 0 |
| 0 | 1 | | 1 |
| 1 | 0 | | 1 |
| 1 | 1 | | 0 |

# Aufgabe 14 - Modulo-Funktion
Eine in der Computertechnik wichtige mathematische Funktion ist die Restwert- oder 
Modulo-Funktion mit dem in z.B. Java und C verwendeten Operationszeichen %. 
Versuchen sie nun die folgende Berechnungen auszuführen. Was stellen sie fest?
- a. 11 % 2 = 1
- b. 10 % 2 = 0
- c. 10 % 3 = 1
- d. 10 % 5 = 0
- e. 10 % 9 = 1

# Reflexion
- Ich habe gerlent wie man Binär addiert und wie man Sie Dezimal darstellt.
- Ich habe gelernt das 4 Bit eine Hexziffer entspricht.
- Ich habe gerlernt was AND, OR, NOT und EXOR ist und welche Ausgaben sie mir geben.
- Ich habe gelernt was das chmod 751 CreateWeeklyReport ist. 

*Heute habe ich vieles dazu gerlernt und mein Wissen expandiert.*