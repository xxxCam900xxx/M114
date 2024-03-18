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

---------------------------------------

### Aufgabe 1
Um ein gewisses Verständnis für die Luminanz-Chrominanz-Beschreibung von 
Farben zu erhalten, lösen sie die folgenden Aufgaben. 
Benutzen sie dazu dieses Online-Tool: https://colorizer.org/

• RGB 255/255/255 entspricht Weiss und ergibt in YCbCr: **Y:1 Cb:0 Cr:0**
• RGB 0/0/0 entspricht Schwarz und ergibt in YCbCr: **Y:0 Cb:0 Cr:0**
• Y:0, Cb:0.5, Cr:0 entspricht der Farbe: **rgb(179, 0, 0)**
• Y:0, Cb:-0.5, Cr:0 entspricht der Farbe: **rgb(0, 91, 0)**
• Y:0, Cb:0, Cr:0.5 entspricht der Farbe: **rgb(0, 0, 226)**
• Y:0, Cb:0, Cr:-0.5 entspricht der Farbe: **rgb(0, 44, 0)**
• Y:0.3, Cb:0.5, Cr:-0.17 entspricht der Farbe: **rgb(255, 0, 0)**

### Aufgabe 2
Ein RGB-Farbbild benutzt nur die Farbe Weiss als Hintergrund und ein Hellblau mit 
folgenden Werten: R=33, G=121, B=239 (8 Bit pro Farbkanal). Das Bild soll in ein 
Graustufenbild umgewandelt werden. 

Berechnen sie den für das Hellblau entsprechende Grauwert. (8 Bit pro Farbkanal)

- G: 121 => 60% => **73**
- R: 33 => 30% => **10**
- B 239 => 10% => **24**

### Aufgabe 3
Berechnen sie, wieviel Speicher eingespart wird, wenn ein Bild mit Subsampling 4:1:1 komprimiert wird.

- R = 100%
- G = 25%
- B = 25%

1000bits gespart, da  R_1000 +  G_500 + B_500 = **2000**

### Aufgabe 4
Der folgende Youtube-Film beschäftigt sich mit RGB und YCrCb:
https://www.youtube.com/watch?v=3dET-EoIMM8
Schauen sie den an und beantworten sie anschliessend diese Fragen:

- a. Kann man durch die Bildumwandlung vom RGB- in den YCbCr-Farbraum 
Speicherplatz einsparen?
- b. Kann ein Beamer ein Bikld im YCbCr-Farbbereich darstellen?
- c. Wie rechnet man ein Farbbildes in ein Graustufenbild um?
- d. Warum hat bei der Umwandlung eine Farbbildes in ein Graustufenbild der 
Grünanteil am meisten Gewicht?

a. Ja, durch die Bildumwandlung vom RGB- in den YCbCr-Farbraum kann Speicherplatz eingespart werden. Im RGB-Farbraum werden die Farbinformationen für jeden einzelnen Pixel separat in Form von drei Farbkanälen (Rot, Grün und Blau) gespeichert. Durch die Umwandlung in den YCbCr-Farbraum werden die Farbinformationen in einen Helligkeitskanal (Y) und zwei Chrominanzkanäle (Cb und Cr) aufgeteilt. Da das menschliche Auge empfindlicher für Helligkeitsänderungen als für Farbänderungen ist, können die Chrominanzkanäle mit einer geringeren Auflösung (z. B. durch Subsampling) gespeichert werden, während die Helligkeitsinformationen mit höherer Genauigkeit beibehalten werden. Dies führt zu einer Reduzierung des Speicherbedarfs für die Farbinformationen.

b. Ja, ein Beamer kann ein Bild im YCbCr-Farbbereich darstellen. Der YCbCr-Farbraum ist ein gängiger Farbraum in der Videotechnik, der speziell für die digitale Darstellung und Übertragung von Bildern und Videos entwickelt wurde. Die meisten digitalen Video- und Bildformate verwenden den YCbCr-Farbraum, um Farbinformationen effizient zu codieren und darzustellen. Ein Beamer kann diese Informationen decodieren und das Bild entsprechend anzeigen.

c. Um ein Farbbild in ein Graustufenbild umzurechnen, kann man verschiedene Methoden verwenden. Eine gängige Methode ist die Berechnung eines gewichteten Durchschnitts der Farbkanäle. Dabei werden die Farbwerte der einzelnen Pixel (normalerweise im RGB-Farbraum) gewichtet und zu einem Grauwert kombiniert. Eine häufig verwendete Gewichtung ist die sogenannte "Luminanz-Methode", bei der die Gewichtung der Farbkanäle basierend auf ihrer Wahrnehmungsrelevanz angepasst wird. Für den RGB-Farbraum lautet die Formel:

Grauwert = 0,2989 * Rot + 0,5870 * Grün + 0,1140 * Blau

d. Bei der Umwandlung eines Farbbildes in ein Graustufenbild hat der Grünanteil am meisten Gewicht, weil das menschliche Auge für die grüne Farbe am empfindlichsten ist. Das menschliche visuelle System ist besonders gut darin, kleinste Unterschiede in den grünen Farbtönen wahrzunehmen. Daher wird der Grünkanal mit einem höheren Gewicht in die Berechnung des Grauwerts einbezogen, um eine bessere Wahrnehmung der Helligkeitsunterschiede im Graustufenbild zu ermöglichen. Die spezifischen Gewichtungsfaktoren können je nach Anwendung variieren, aber in der Regel wird der Grünkanal am stärksten gewichtet, gefolgt von Rot und Blau.

### Aufgabe 5
Der folgende Youtube-Film beschäftigt sich mit Chroma-Subsampling:
https://www.youtube.com/watch?v=Nd-7o3o5x6A
Schauen sie den an und beantworten sie anschliessend diese Fragen:

- a. Warum verschlechtert sich die Bildschärfe von 4:1:1-Subsampling gegenüber 
4:4:4-Subsampling nicht?
- b. Ein quadratisches 24-Bit-RGB-Bild mit einer Kantenlänge von 1000 Pixel soll 
mit 4:1:1 unterabgetatstet werden. Wieviel Speicherplatz wird damit 
eingespart?

a. Die Bildschärfe verschlechtert sich bei 4:1:1-Subsampling im Vergleich zu 4:4:4-Subsampling, da bei 4:1:1-Subsampling die Farbinformationen reduziert werden. Bei 4:4:4-Subsampling werden alle Farbinformationen für jeden einzelnen Pixel gespeichert, während bei 4:1:1-Subsampling nur für eine Gruppe von vier Pixeln ein Farbwert gespeichert wird. Dies bedeutet, dass bei 4:1:1-Subsampling die Farbinformationen nur mit einer geringeren Auflösung vorhanden sind, was zu einem Verlust an Detailgenauigkeit und Bildschärfe führen kann. Insbesondere bei feinen Farbübergängen und Texturen kann es zu einem sichtbaren Qualitätsverlust kommen.

b. Bei 4:1:1-Subsampling wird für eine Gruppe von vier Pixeln nur ein Farbwert gespeichert, während die Helligkeitswerte für alle vier Pixel beibehalten werden. Wenn das ursprüngliche Bild ein 24-Bit-RGB-Bild mit einer Kantenlänge von 1000 Pixeln ist, berechnet sich der Speicherplatzbedarf wie folgt:

Ursprünglicher Speicherplatzbedarf = (1000 * 1000) * 3 Byte

Beim 4:1:1-Subsampling werden nur 1/4 der Farbwerte gespeichert, während die Helligkeitswerte weiterhin 3 Byte pro Pixel belegen. Daher ergibt sich der neue Speicherplatzbedarf wie folgt:

Neuer Speicherplatzbedarf = (1000 * 1000 / 4) * (1 Byte + 3 Byte)

Speichereinsparung = Ursprünglicher Speicherplatzbedarf - Neuer Speicherplatzbedarf

Bitte beachten Sie, dass 1 Byte für den Farbwert und 3 Byte für die Helligkeitswerte angenommen wurden, was von der tatsächlichen Implementierung und dem verwendeten Dateiformat abhängen kann.

### Aufgabe 6
Der folgende Youtube-Film beschäftigt sich mit der JPG-Komprimierung:
https://www.youtube.com/watch?v=Kv1Hiv3ox8I
Schauen sie den an und beantworten sie anschliessend diese Fragen:

- a. Was ist der erste Schritt bei der JPG-Komprimierung?
- b. Führt die DCT-Transformation zu einer Datenreduktion?
- c. Warum erhält man bei einer sehr starken Bildkomprimierung sogenannte 
Block-Artefakte

a. Der erste Schritt bei der JPEG-Komprimierung ist die Umwandlung des Bildes vom RGB- in den YCbCr-Farbraum. Dieser Farbraum ermöglicht eine effizientere Komprimierung, da die menschliche Wahrnehmung von Helligkeit und Farbe unterschiedlich ist. Durch die Umwandlung in den YCbCr-Farbraum werden die Farbinformationen von der Helligkeitsinformation getrennt, was es ermöglicht, die Farbinformationen mit geringerer Auflösung zu speichern und somit Speicherplatz zu sparen.

b. Ja, die DCT (Diskrete Cosinus Transformation)-Transformation führt zu einer Datenreduktion. Die DCT-Transformation wird angewendet, um das Bild in den Frequenzbereich zu überführen. Dabei werden die Bildinformationen in Form von Koeffizienten dargestellt, die die verschiedenen Frequenzkomponenten im Bild repräsentieren. Die DCT ist eine verlustfreie Transformation, die es ermöglicht, die Energiekonzentration der Bildinformationen zu komprimieren. Durch die DCT-Transformation werden die hochfrequenten Komponenten reduziert und die niedrigfrequenten Komponenten beibehalten. Da das menschliche Auge weniger empfindlich auf hochfrequente Informationen reagiert, können diese mit geringerer Genauigkeit gespeichert werden. Dadurch wird die Datenmenge des Bildes reduziert.

c. Bei einer sehr starken Bildkomprimierung können sogenannte Block-Artefakte auftreten. Dies liegt daran, dass JPEG ein verlustbehaftetes Kompressionsverfahren ist und bei hoher Kompressionsrate Informationen verloren gehen. Das Bild wird in Blöcke aufgeteilt und diese Blöcke werden unabhängig voneinander komprimiert. Wenn die Kompressionsrate sehr hoch ist, werden feine Details und Texturen stark reduziert oder sogar entfernt. Dies führt zu sichtbaren Artefakten, die als Block-Artefakte bezeichnet werden. Block-Artefakte äußern sich in Form von sichtbaren Kanten zwischen den Blöcken und Unregelmäßigkeiten in flachen Bereichen des Bildes. Die Stärke der Block-Artefakte hängt von der Kompressionsrate und den spezifischen Komprimierungseinstellungen ab.

### Aufgabe 7
Der folgende Youtube-Film beschäftigt sich mit Codecs und Containern:
https://www.youtube.com/watch?v=-4NXxY4maYc
Schauen sie den an und beantworten sie anschliessend diese Fragen:

- a. Was ist der Unterschied zwischen Intraframe- und InterframeKomprimierung?
- c. Bei welcher Filmsequenz bietet die Interframekomprimierung mehr Potential
zur Datenreduzierung:
  - i. 30 Sekunden-Szene mit Faultier auf Nahrungssuche?
  - ii. 30 Sekunden-Szene mit Zieleinfahrt beim Formel-1-Rennen?
- d. Sehen sie Parallelen zwischen Datenbackupkonzepten und InterframeKomprimierung?
- e. Was versteht man unter GOP25

a. Die Intraframe-Komprimierung und die Interframe-Komprimierung sind zwei verschiedene Methoden der Videokomprimierung.

Die Intraframe-Komprimierung, auch bekannt als Frame-Komprimierung oder I-Komprimierung, komprimiert jedes Einzelbild (Frame) in einem Video unabhängig voneinander. Bei dieser Methode werden die Daten innerhalb jedes Frames reduziert, indem redundante Informationen entfernt oder durch kompaktere Darstellungen ersetzt werden. Jedes Frame wird als eigenständiges Bild betrachtet, ohne Bezug zu anderen Frames in der Videosequenz.

Die Interframe-Komprimierung hingegen basiert auf der Ausnutzung der Redundanz zwischen aufeinanderfolgenden Frames in einer Videosequenz. Hierbei werden nicht nur die Einzelbilder komprimiert, sondern auch die Unterschiede (Bewegungsvektoren) zwischen den Frames analysiert und codiert. Statt jedes Frame vollständig zu speichern, werden nur die Änderungen zwischen den Frames gespeichert. Dadurch kann eine höhere Kompressionsrate erreicht werden, da sich viele Teile der Videosequenz über mehrere Frames hinweg nicht ändern.

c. Bei der 30-Sekunden-Szene mit dem Faultier auf Nahrungssuche bietet die Interframe-Komprimierung wahrscheinlich mehr Potential zur Datenreduzierung. In einer solchen Szene bewegt sich das Faultier normalerweise sehr langsam, und es gibt wahrscheinlich viele Frames, in denen sich die Bildinformationen nur minimal ändern. Die Interframe-Komprimierung kann die Änderungen zwischen den Frames effizient kodieren und redundante Informationen reduzieren, da sich viele Teile des Bildes über mehrere Frames hinweg nicht ändern.

Im Gegensatz dazu enthält eine 30-Sekunden-Szene mit der Zieleinfahrt beim Formel-1-Rennen wahrscheinlich eine schnellere Bewegung und häufige Änderungen in den Bildinformationen von Frame zu Frame. In solchen Szenen kann die Intraframe-Komprimierung effektiver sein, da jedes Frame als eigenständiges Bild betrachtet wird und keine signifikanten Redundanzen zwischen den aufeinanderfolgenden Frames vorhanden sind.

d. Es gibt gewisse Parallelen zwischen Datenbackupkonzepten und Interframe-Komprimierung. Beide Methoden zielen darauf ab, Speicherplatz zu sparen und die Effizienz bei der Speicherung von Daten zu verbessern.

Beim Datenbackup werden häufig inkrementelle oder differentielle Backups verwendet, um nur die Änderungen zwischen verschiedenen Backup-Versionen zu speichern. Ähnlich dazu kodiert die Interframe-Komprimierung nur die Änderungen zwischen aufeinanderfolgenden Frames in einer Videosequenz, anstatt jedes Frame vollständig zu speichern.

Sowohl Datenbackupkonzepte als auch Interframe-Komprimierung nutzen die Redundanz oder Wiederholungen von Daten, um die Datenmenge zu reduzieren. Durch die Speicherung von nur geänderten oder differenziellen Informationen kann sowohl bei Datenbackups als auch bei der Videokomprimierung eine effizientere Nutzung des verfügbaren Speicherplatzes erreicht werden.

e. GOP25 steht für "Group of Pictures 25". Es handelt sich dabei um einen Begriff, der in der Videokomprimierung verwendet wird, insbesondere im Zusammenhang mit dem MPEG-Videoformat.

Eine GOP (Group of Pictures) besteht aus einer Gruppe von aufeinanderfolgenden Frames in einer Videosequenz. Die Zahl 25 in GOP25 gibt die Anzahl der Frames in einer GOP an. In diesem Fall enthält jede GOP 25 Frames.

In einer Videokomprimierung mit einer GOP von 25 Frames würde beispielsweise das 26. Frame die Informationen für das erste Frame der nächsten GOP enthalten. Die Interframe-Komprimierung basiert auf der Kodierung der Unterschiede zwischen Frames innerhalb einer GOP und zwischen GOPs.

Die Wahl der GOP-Größe kann Auswirkungen auf die Kompressionsrate, die Qualität des komprimierten Videos und die Effizienz der Codierung haben. Eine GOP-Größe von 25 Frames ist typisch für das MPEG-Videoformat, wird jedoch je nach Anwendung und Anforderungen variieren können.