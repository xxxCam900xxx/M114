# A_DATEN_CODIEREN_NUM_ANNE

- [Aufgabe 1](https://github.com/CameronMeile/M114/tree/main/19_02%20-%20Week%201#aufgabe-1)
- [Aufgabe 2](https://github.com/CameronMeile/M114/tree/main/19_02%20-%20Week%201#aufgabe-2)

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

911 / 2 = 455 | R-1
455 / 2 = 227 | R-1
227 / 2 = 113 | R-1
113 / 2 = 56  | R-1
56  / 2 = 28  | R-0
28  / 2 = 14  | R-0
14  / 2 = 7   | R-0
7   / 2 = 3   | R-1
3   / 2 = 1   | R-1
1   / 2 = 0   | R-1

=

**1 1 1 1 0 0 0 1 1 1**

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
