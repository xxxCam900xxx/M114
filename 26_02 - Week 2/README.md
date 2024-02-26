# A_DATEN_CODIEREN_TXT_ANNEX

### Inhaltsverzeichnis
- [Aufgabe 1](#aufgabe-1)
- [Aufgabe 2](#aufgabe-2)
- [Aufgabe 3](#aufgabe-3)

---------------------------------------

# Aufgabe 1
Besorgen sie sich im Internet eine vollständige ASCII-Tabelle als Bild- oder 
PDF-Datei und ergänzen sie damit ihr ePortfolio.

### ASCII Tabelle
![ASCII Tabelle](/26_02%20-%20Week%202/Content/ascii-tabelle.gif)
[Übersichtlichere ASCII Tabelle](/26_02%20-%20Week%202/Content/ASCII-Tabelle.pdf)

### ASCII Tabelle Hexadezimal
![ASCII Tabelle Hexadezimal](/26_02%20-%20Week%202/Content/ASCII%20Tabelle%20Hex.png)

# Aufgabe 2
Suchen sie im Internet nach einer Webseite, wo Unicode-Zeichen gelistet sind 
und merken bzw. notieren sie sich den Link.

![Unicode Tabelle](/26_02%20-%20Week%202/Content/Unicode%20Tabelle.png)
- [Unicode Website](https://www.compart.com/de/unicode/category/So)
- [Unicode Wikipedia](https://de.wikipedia.org/wiki/Unicodeblock_Verschiedene_Symbole)
# Aufgabe 3
Sie erhalten eine ZIP-Datei Textsamples.zip unter folgendem Link: 
https://juergarnold.ch/Codesysteme/Textsamples.zip
Laden sie die ZIP-Datei auf ihren Notebook und extrahieren sie die drei Dateien 
Textsample1, Textsample2 und Textsample3. Eine der drei Dateien ist in 
ASCII codiert, die andere in UTF-8 und die dritte in UTF-16. Beantworten sie nun die 
folgenden Fragen:
### a. 
Welche der Dateien ist nun ASCII-codiert, welche UTF-8 und welche UTF-16 
BE-BOM?
- ANSI / ASCII = [Textsample 1](/26_02%20-%20Week%202/Content/Textsample1)
- UTF-8 = [Textsample 2](/26_02%20-%20Week%202/Content/Textsample2)
- UTF-16 BE BOM = [Textsample 3](/26_02%20-%20Week%202/Content/Textsample3)
### b. 
Alle drei Dateien enthalten denselben Text. Aus wie vielen Zeichen besteht 
dieser?
- Die Text Länge / Anzahl zeichen besteht aus **71 Zeichen**.
### c. 
Was sind die jeweiligen Dateigrössen? (Beachten sie, dass unter Grösse auf 
Datenträger jeweils 0 Bytes angegeben wird. Dies darum, weil beim WindowsDateisystem NTFS kleine Dateien direkt in die MFT (Master File Table) 
geschrieben werden.) Wie erklären sie sich die Unterschiede?
- [Textsample 1](/26_02%20-%20Week%202/Content/Textsample1) - 68 Bytes
- [Textsample 2](/26_02%20-%20Week%202/Content/Textsample2) - 71 Bytes
- [Textsample 3](/26_02%20-%20Week%202/Content/Textsample3) - 138 Bytes
##### Mögliche Unterschiede
**Dateisystem-Overhead**: Das Dateisystem selbst kann zusätzlichen Overhead-Speicherplatz benötigen, um Metadaten und andere Informationen über die Dateien zu speichern. Dieser Overhead kann von Dateisystem zu Dateisystem variieren und zu geringfügigen Unterschieden in den angezeigten Dateigrößen führen.

**Speicherplatz-Clustergrösse**: Das Dateisystem organisiert den Speicherplatz in Clustern, wodurch die kleinste zu belegende Speichereinheit festgelegt wird. Wenn die Clustergröße größer ist als die tatsächliche Dateigröße, wird der gesamte Cluster für die Speicherung der Datei reserviert, was zu einem Verschwendungs von Speicherplatz führen kann. Dies kann zu geringfügig größeren Dateigrößen führen.

**Dateikompression**: Einige Dateisysteme oder Komprimierungsalgorithmen können kleine Dateien automatisch komprimieren, um Speicherplatz zu sparen. Dadurch kann die tatsächliche Größe auf dem Datenträger kleiner sein als die ursprüngliche Dateigröße.
### d. 
Bei den weiteren Fragen interessieren uns nur noch die ASCII- und die UTF8-Datei: Bekanntlich ist UTF-8 in den ersten 128 Zeichen deckungsgleich mit 
ASCII. Untersuchen sie nun die beiden HEX-Dumps und geben sie an, welche 
Zeichen unterschiedlich codiert sind. Ein kleiner Tipp: Es sind deren zwei.
##### ASCII-HEX-Dump:
50 61 72 69 74 61 74 20 53 63 68 77 65 69 7A 65 72 2D 46 72 61 6E 6B 65 6E 20 7A 75 20 45 75 72 6F 20 62 65 64 65 75 74 65 74 3A 20 31 30 30 43 48 46 20 65 6E 74 73 70 72 65 63 68 65 6E 20 31 30 30 E2 82 AC

##### UTF-8-HEX-Dump:
50 61 72 C3 A4 74 69 74 20 53 63 68 77 65 69 7A 65 72 2D 46 72 61 6E 6B 65 6E 20 7A 75 20 45 75 72 6F 20 62 65 64 65 75 74 65 74 3A 20 31 30 30 43 48 46 20 65 6E 74 73 70 72 65 63 68 65 6E 20 31 30 30 E2 82 AC

#### Unterschiede
Das Zeichen "**ä**"
- ASCII = **E4**
- UTF-8 = **C3 A4**

Das Euro-Zeichen "**€**" 
- ASCII = **80**
- UTF-8 = **E2 82 AC**
### e. 
Was bedeuten die beiden Ausdrücke, denen wir z.B. bei UTF-16 begegnen: 
Big-Endian (BE), Little-Endian (LE)?
##### BE: Big-Endian
Das höchstwertigste Byte wird zuerst, bzw. an der kleinsten Speicheradresse gespeichert. Die grösstwertigste Komponente wird zuerst genannt, wie z.B. bei der Uhrzeit: Stunde.Minute.
##### LE: Little-Endian
Das kleinstwertigste Byte wird an der Anfangsadresse gespeichert, also die kleinstwertige Komponente zuerst genannt, wie z.B. beim Datum: Monat.Jahr.
### f. 
Im Notepad++ kann man unter dem Menüpunkt Codierung von ASCII zu UTF 
umschalten. Spielen sie damit etwas herum und notieren sie sich, was in der 
Darstellung jeweils ändert. 
### g.
Für Anspruchsvolle: Der UTF-8-Code kann je nach Zeichen ein, zwei, drei 
oder vier Byte lang sein. Wie kann der Textreader erkennen, wann ein UTF-8 
Zeichencode beginnt und wann er endet? Untersuchen sie dies anhand der 
beiden Textsamples und lesen sie in z.B. Wikipedia die entsprechende 
Theorie zu UTF-8 durch. Tipp: Startbyte und Folgebyte.

# Aufgabe 4
Denken sie sich eine kurze Botschaft, URL etc. aus und bilden sie diese Information 
in einem QR-Code ab. Danach tauschen sie mit ihrem Banknachbar/in ihre QRCodes aus. Wenn der QR-Code gelesen werden kann, waren sie erfolgreich. 
Applikationen die alphanumerischen Text in einen QR-Code und zurück wandeln, 
findet man im Internet. 

![QR-CODE](/26_02%20-%20Week%202/Content/QR-Code.svg)

# Aufgabe 5
Ihre Firma wird mit dem Design von Tickets für ein Fussballstadion beauftragt. Das 
Eintrittsticket soll mit einem QR-Code versehen sein, der alle wichtigen Informationen 
zur Buchung enthält. Dies soll ermöglichen, das Ticket jederzeit und überall von 
Offline-QR-Readern lesen und überprüfen zu lassen bzw. Zugang zu den 
Stadionbereichen zu gewähren. Das Ticket soll die folgenden, codierten 
Informationen enthalten: 
### a. Datum und Uhrzeit der Veranstaltung
### b. Fortlaufende, alphanumerische Ticketnummer (Ticketnummern seit Tag-0)
### c. Numerische Sitzplatznummer (Jeder Sitzplatz hat eigene Nummer)
### d. Tribünensektor A-Z (Für einfache Platzeinweisung der Besucher)
### e. ID- oder Passnummer des Besuchers (Tickets nicht übertragbar)
- Überlegen sie sich, ob das Ticket fälschungssicher ist. Braucht es allenfalls 
noch eine Prüfziffer, Checksum etc.?
- Wenn der Besucher am Stadioneingang erscheint, zeigt er sein Ticket. Dieses 
wird von einem Platzanweiser mit einem QR-Code-Leser gelesen. Damit kann 
er die Personalie und Gültigkeit des Tickets überprüfen und den Besucher 
anschliessend in den richtigen Stadionsektor leiten.
- Bilden sie diesen Datensatz in einen QR-Code ab. Erstellen sie QR-Codes für 
fiktive Veranstaltungen. Testen sie ihre QR-Codes mit ihrem Banknachbarn/in 
gegenseitig aus.
- Applikationen die alphanumerischen Text in einen QR-Code und zurück 
wandeln, findet man im Internet.
- Auf Komplettlösungen aus dem Internet - es gibt zu diesem Thema mehr oder 
weniger "pfannenfertige" Applikationen - bitte aber verzichten.