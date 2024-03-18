# 11.03 - Week 4

### Inhaltsverzeichnis
- [11.03 - Week 4](#1103---week-4)
    - [Inhaltsverzeichnis](#inhaltsverzeichnis)
- [Aufgabe 1](#aufgabe-1)
- [Aufgabe 2](#aufgabe-2)
- [Aufgabe 3](#aufgabe-3)
- [Aufgabe 4](#aufgabe-4)
- [Aufgabe 5](#aufgabe-5)
- [Aufgabe 6](#aufgabe-6)
- [Aufgabe 7](#aufgabe-7)
- [Aufgabe 8](#aufgabe-8)
- [Aufgabe 9](#aufgabe-9)
    - [RAW-Format:](#raw-format)
    - [Verwendungszwecke des RAW-Formats:](#verwendungszwecke-des-raw-formats)
    - [JPG-Format:](#jpg-format)
    - [Verwendungszwecke des JPG-Formats:](#verwendungszwecke-des-jpg-formats)
- [18.03 - Week 5](#1803---week-5)
    - [Aufgabe 10](#aufgabe-10)

---------------------------------------

# Aufgabe 1
Bestimmen sie die Farben für die folgenden RGB-Farbcodes (in DEZ und HEX). 
Nutzen sie den RGB-Farbenmixer. Benutzern sie dazu die beiden Online-Tools:
[w3Scools - Hexdecimal.asp](https://www.w3schools.com/colors/colors_hexadecimal.asp)
[w3Scools - RGB.asp](https://www.w3schools.com/colors/colors_rgb.asp)

- RGB(255, 255, 255) entspricht Farbe: **Weiss**
- RGB(0,0,0) entspricht Farbe: **Schwarz**
- RGB(252,178,91) entspricht Farbe: **Orange**
- #FF0000 entspricht Farbe: **Rot**
- #00FF00 entspricht Farbe: **Limetten Grün**
- #0000FF entspricht Farbe: **Blau**
- #FFFF00 entspricht Farbe: **Gelb**
- #00FFFF entspricht Farbe: **Cyan**
- #FF00FF entspricht Farbe: **Magenta**
- #000000 entspricht Farbe: **Schwarz**
- #FFFFFF entspricht Farbe: **Weiss**
- #00BC00 entspricht Farbe: **Grün**

# Aufgabe 2
Bestimmen sie die Farben für die folgenden prozentualen CMYK-Angaben. Nutzen 
sie den CMYK-Farbenmixer bzw. das folgende Online-Tool:
[w3Scools - CMYK.asp](https://www.w3schools.com/colors/colors_cmyk.asp)

- C:0%, M:100%, Y:100%, K:0% entspricht Farbe: **Rot**
- C:100%, M:0%, Y:100%, K:0% entspricht Farbe: **Limetten Grün**
- C:100%, M:100%, Y:0%, K:0% entspricht Farbe: **Blau**
- C:0%, M:0%, Y:100%, K:0% entspricht Farbe: **Gelb**
- C:100%, M:0%, Y:0%, K:0% entspricht Farbe: **Cyan**
- C:0%, M:100%, Y:0%, K:0% entspricht Farbe: **Magenta**
- C:100%, M:100%, Y:100%, K:0% entspricht Farbe: **Schwarz**
- C:0%, M:0%, Y:0%, K:100% entspricht Farbe: **Schwarz**
- C:0%, M:0%, Y:0%, K:0% entspricht Farbe: **Weiss**
- C:0%, M:46%, Y:38%, K:22% entspricht Farbe: **Altrosa**

# Aufgabe 3
Berechnen sie den theoretischen Speicherbedarf in Bit und in Byte eines unkomprimierten RGB-Bildes mit der Grösse 640 x 480 und 8Bit Auflösung pro Farbkanal.

Gegeben:
- Auflösung: 640 x 480 Pixel
- Farbtiefe pro Kanal: 8 Bit
- 2^8 = 256

Der Speicherbedarf pro Pixel beträgt also 8 Bit für den roten Kanal + 8 Bit für den grünen Kanal + 8 Bit für den blauen Kanal = 24 Bit (oder 3 Byte).

640 Pixel * 480 Pixel = 307,200 Pixel
307,200 Pixel * 24 Bit pro Pixel = 7,372,800 Bit

Um den Speicherbedarf in Byte zu erhalten, teilen wir den Speicherbedarf in Bit durch 8:

7,372,800 Bit / 8 = 921,600 Byte

Also beträgt der theoretische Speicherbedarf eines unkomprimierten RGB-Bildes mit der Größe 640 x 480 und 8 Bit Auflösung pro Farbkanal 7,372,800 Bit oder 921,600 Byte.

# Aufgabe 4
Sie müssen die Webseite der Firma Muster-GmbH gestalten. Als Hintergrundbild (background-image) soll eine gekachelte Textur verwendet werden. (background-repeat: repeat). Auf diesen Hintergrund wird das Firmenlogo gelegt. 
![MusterGmbH](/11_03%20-%20Week%204/Content/MusterGMBH.png)
Für welche Bildformate werden sie sich entscheiden? Begründen sie! **1200x800**

# Aufgabe 5
Sie haben ein 30-Zoll-Display (Diagonale) im Format 16:10 und 100ppi erworben. Was ist die Pixelauflösung horizontal und vertikal?

Höhe = Diagonale * (10 / √(16² + 10²))
Höhe = 30 * (10 / √(256 + 100))
Höhe = 30 * (10 / √356)
Höhe ≈ 30 * (10 / 18.87)
Höhe ≈ 30 * 0.5297
Höhe ≈ 15.89 Zoll

Breite = Höhe * (16 / 10)
Breite ≈ 15.89 * (16 / 10)
Breite ≈ 25.42 Zoll

Horizontale Pixelauflösung = Breite * PPI
Horizontale Pixelauflösung ≈ 25.42 * 100
Horizontale Pixelauflösung ≈ 2542 Pixel
Vertikale Pixelauflösung = Höhe * PPI
Vertikale Pixelauflösung ≈ 15.89 * 100
Vertikale Pixelauflösung ≈ 1589 Pixel

**2542x1589**

# Aufgabe 6
Sie drucken ein quadratisches Foto mit einer Kantenlänge von 2000 Pixel mit 600dpi. Wie gross in cm wird dieses?

Gegeben:
- Kantenlänge des Fotos: 2000 Pixel
- Auflösung: 600 dpi
- 1 Zoll entspricht 2,54 cm.

**Größe des Fotos in cm = (Kantenlänge des Fotos / Auflösung) * Umrechnungsfaktor**

Größe des Fotos in cm = (2000 Pixel / 600 dpi) * 2,54 cm/Zoll
Größe des Fotos in cm = (2000 / 600) * 2,54 cm
Größe des Fotos in cm = 3,333 * 2,54 cm
Größe des Fotos in cm ≈ 8,47 cm

# Aufgabe 7
Berechnen sie den Speicherbedarf für ein unkomprimiertes Einzelbild im HD1080p50-Format bei einer True-Color-Farbauflösung.

Gegeben:
- Breite = 1920 Pixel
- Höhe = 1080 Pixel

**Anzahl der Pixel im Bild = Breite x Höhe**

Anzahl der Pixel im Bild = 1920 x 1080 = 2,073,600 Pixel
Da jeder Pixel mit 24 Bit Farbtiefe dargestellt wird, benötigen wir 24 Bit pro Pixel.
Speicherbedarf für ein Einzelbild = Anzahl der Pixel im Bild x Farbtiefe
Speicherbedarf für ein Einzelbild = 2,073,600 Pixel x 24 Bit
Speicherbedarf für ein Einzelbild = 49,766,400 Bit

Um den Speicherbedarf in Byte umzurechnen, teilen wir den Wert durch 8:
- Speicherbedarf für ein Einzelbild = 49,766,400 Bit / 8 = 6,220,800 Byte

Um den Speicherbedarf in Megabyte (MB) umzurechnen, teilen wir den Wert durch 1,048,576 (da 1 Megabyte = 1,048,576 Byte):

- Speicherbedarf für ein Einzelbild = 6,220,800 Byte / 1,048,576 = 5.9375 MB

Der Speicherbedarf für ein unkomprimiertes Einzelbild im HD1080p50-Format bei True-Color-Farbauflösung beträgt etwa 5,9375 Megabyte.

# Aufgabe 8
Welchen Speicherbedarf aus einer HD (Massvorsatz im IEC-Format) hat das Video aus der vorangegangenen Aufgabe bei einer Spieldauer von 3 Minuten?

Gegeben:
- 5,9375 Megabyte
- 50 Bildern pro

**Anzahl der Bilder = Bildwiederholrate (Bilder pro Sekunde) x Dauer (in Sekunden)**

Bildwiederholrate = 50 Bilder pro Sekunde
Dauer = 3 Minuten = 3 x 60 Sekunden = 180 Sekunden
Anzahl der Bilder = 50 x 180 = 9,000 Bilder

Um den Speicherbedarf des Videos zu berechnen, multiplizieren wir den Speicherbedarf pro Einzelbild mit der Anzahl der Bilder:

**Speicherbedarf des Videos = Speicherbedarf pro Einzelbild x Anzahl der Bilder**

Speicherbedarf des Videos = 5,9375 Megabyte x 9,000
Speicherbedarf des Videos ≈ 53,437.5 Megabyte

Der Speicherbedarf des Videos bei einer Spieldauer von 3 Minuten beträgt ungefähr 53,437.5 Megabyte.

# Aufgabe 9
Ihre Digitalkamera bietet für die Speicherung ihrer Bilder die beiden Formate RAW und JPG an. Wo liegen die Unterschiede und was sind die Verwendungszwecke?.

### RAW-Format:
- RAW ist ein unkomprimiertes Dateiformat, das alle Rohdaten, die von der Kamera erfasst wurden, speichert.
- Es enthält alle Bildinformationen, die von den Bildsensoren erfasst wurden, ohne jegliche interne Verarbeitung oder Komprimierung.
- RAW-Dateien bieten eine höhere Flexibilität bei der Nachbearbeitung, da sie mehr Spielraum für Belichtungskorrekturen, Weißabgleichsanpassungen und andere Einstellungen bieten.
- Sie ermöglichen eine verlustfreie Bearbeitung der Bilder, da sie keine Komprimierung oder Datenreduktion enthalten.
- RAW-Dateien sind in der Regel größer als JPG-Dateien, da sie mehr Speicherplatz für die Speicherung der unverarbeiteten Bilddaten benötigen.
- Das RAW-Format erfordert spezielle Software oder RAW-Konverter, um die Dateien in ein bearbeitbares oder druckbares Format 

### Verwendungszwecke des RAW-Formats:

- Professionelle Fotografen und fortgeschrittene Hobbyisten verwenden oft das RAW-Format, um die maximale Kontrolle über ihre Bilder und eine umfassende Nachbearbeitung zu haben.
- Es wird empfohlen, RAW zu verwenden, wenn man in schwierigen Lichtsituationen arbeitet, wo eine genaue Belichtungskorrektur erforderlich ist.
- Wenn man die Endbearbeitung der Bilder selbst durchführen möchte, bietet das RAW-Format die beste Flexibilität und Qualität.umzuwandeln.

### JPG-Format:
- JPG ist ein komprimiertes Dateiformat, das eine verlustbehaftete Komprimierung verwendet, um die Dateigröße zu reduzieren.
- Bei der Komprimierung gehen bestimmte Bildinformationen verloren, was zu einem geringen Qualitätsverlust führen kann. Die Komprimierung kann Artefakte wie Blockbildung oder Schärfeverluste verursachen.
- JPG-Dateien sind in der Regel kleiner als RAW-Dateien und nehmen weniger Speicherplatz ein.
- Die meisten Kameras bieten verschiedene Qualitätsstufen für JPG-Dateien an, um die Dateigröße anzupassen und die Bildqualität zu beeinflussen.
- JPG-Dateien sind sofort einsatzbereit und können direkt aus der Kamera geteilt, gedruckt oder online veröffentlicht werden.

### Verwendungszwecke des JPG-Formats:

- JPG wird häufig für den allgemeinen Gebrauch verwendet, wo eine sofortige Verwendung der Bilder ohne umfangreiche Bearbeitung erforderlich ist.
- Es eignet sich gut für den schnellen Austausch von Bildern über soziale Medien, E-Mails oder Online-Galerien.
- JPG wird oft von Hobbyfotografen oder Gelegenheitsnutzern gewählt, die weniger Zeit für die Nachbearbeitung aufwenden möchten.

# 18.03 - Week 5

### Aufgabe 10
Sie möchten ihr neulich erstelltes Gameplay-Video auf Youtube veröffentlichen. Was sind die technischen Vorgaben dazu? (Format, Bildrate, Farbauflösung, Video-, Audiocodec etc.). Gibt es allenfalls rechtliche Einschränkungen?