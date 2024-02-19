# A_DATEN_CODIEREN_NUM_ANNE

- [Aufgabe 1](https://github.com/CameronMeile/M114/tree/main/19_02%20-%20Week%201#aufgabe-1)
- [Aufgabe 2](https://github.com/CameronMeile/M114/tree/main/19_02%20-%20Week%201#aufgabe-2)
- [Aufgabe 3](https://github.com/CameronMeile/M114/tree/main/19_02%20-%20Week%201#aufgabe-3)
- [Aufgabe 4](https://github.com/CameronMeile/M114/tree/main/19_02%20-%20Week%201#aufgabe-4)
- [Aufgabe 5](https://github.com/CameronMeile/M114/tree/main/19_02%20-%20Week%201#aufgabe-5)
- [Aufgabe 6](https://github.com/CameronMeile/M114/tree/main/19_02%20-%20Week%201#aufgabe-6)
- [Aufgabe 7](https://github.com/CameronMeile/M114/tree/main/19_02%20-%20Week%201#aufgabe-7)
- [Aufgabe 8](https://github.com/CameronMeile/M114/tree/main/19_02%20-%20Week%201#aufgabe-8)




---------------------------------------

# Aufgabe 1
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

# Aufgabe 2
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

# Aufgabe 3
Wandeln sie die folgende Binärzahl ohne Taschenrechner in die entsprechende 
Dezimalzahl um: 1011'0110

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| 1 | 0 | 1 | 1 | 0 | 1 | 1 | 0 |

128 + 32 + 16 + 4 + 2 = **182**

# Aufgabe 4
Wandeln sie die folgende Binärzahl ohne Taschenrechner in die entsprechende 
Hexadezimalzahl um: **1110'0010'1010'0101**

| 8 | 4 | 2 | 1 | | 8 | 4 | 2 | 1 | | 8 | 4 | 2 | 1 | | 8 | 4 | 2 | 1 |  
| - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - | - |  
| 1 | 1 | 1 | 0 | - | 0 | 0 | 1 | 0 | - | 1 | 0 | 1 | 0 | - | 0 | 1 | 0 | 1 |  
| **E** | - | - | - | - | **2** | - | - | - | - | **A** | - | - | - | - | **5** | - | - | - |  

# Aufgabe 5
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

# Aufgabe 6 
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

# Aufgabe 7
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

# Aufgabe 8
Dimensionieren sie für den Matterhorn-Express, wo insgesamt 107 Gondeln die 
Touristen von Zermatt auf den Trockenen-Steg befördern, die Codebreite des 
Binärcodes für die Kabinenzählung?

Um die Codebreite des Binärcodes für die Kabinenzählung im Matterhorn-Express zu bestimmen, müssen wir die Anzahl der Gondeln (107) in binärer Form darstellen und die Anzahl der Bits zählen.

Die nächsthöhere Potenz von 2, die größer oder gleich 107 ist, ist 128 (2^7). Das bedeutet, dass wir mindestens 7 Bits benötigen, um 107 Gondeln zu repräsentieren. Die Binärdarstellung von 107 ist 1101011.

Da wir 7 Bits benötigen, um die Kabinenzählung zu codieren, beträgt die Codebreite des Binärcodes 7.


# Aufgabe 13
Erstellen sie die Wahrheitstabellen für die folgenden Funktionen:
- a. Logisch UND/AND (mit zwei Eingangs- und einer Ausgangsvariablen)
- b. Logisch ODER/OR (mit zwei Eingangs- und einer Ausgangsvariablen)
- c. Logisch NICHT/NOT (mit einer Eingangs- und einer Ausgangsvariablen)
- d. Logisch EXOR (mit zwei Eingangs- und einer Ausgangsvariablen)