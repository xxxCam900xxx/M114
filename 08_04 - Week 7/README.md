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
    - [Aufgabe 10](#aufgabe-10)
    - [Aufgabe 11](#aufgabe-11)
    - [Aufgabe 12](#aufgabe-12)
    - [Aufgabe 13](#aufgabe-13)

---------------------------------------

### Aufgabe 1
Wie kann ich einen Public-Key verifizieren?

Um einen Public-Key zu verifizieren, solltest du folgende Schritte beachten:

1. Überprüfe die Quelle des Public-Keys.
2. Vergleiche den Fingerabdruck des Public-Keys mit einer vertrauenswürdigen Quelle.
3. Nutze eine Web-of-Trust, um den Public-Key von anderen vertrauenswürdigen Personen bestätigen zu lassen.
4. Überprüfe, ob der Public-Key von einer Zertifizierungsstelle signiert wurde.
5. Erhalte den Public-Key über einen sicheren Kanal, um Manipulationen zu vermeiden.

Diese Schritte erhöhen die Wahrscheinlichkeit, dass der Public-Key echt ist, bieten jedoch keine absolute Sicherheit.

### Aufgabe 2
Was versteht man unter Public Key Infrastruktur (PKI)?

So sicher asymmetrische Verschlüsselungsverfahren auch sein mögen, wirklich geschützt ist man nur, wenn man dem ausgewählten Public-Key auch vertrauen kann. Das heisst, dass z.B. der Public-Key von Bob auch wirklich Bob gehört und nicht ein mit Bob beschrifteter Public-Key von Mallory ist. Um dies sicherzustellen, muss entweder eine Art Vertrauensnetz aufgebaut werden, oder die Public/Private-Keys werden von offiziellen Stellen, ähnlich den 
Passbüros, ausgestellt. Diese Zertifizierungsstellen klären vor der Schlüsselausgabe die Identität des Antragstellers (mehr oder weniger) seriös ab und garantieren danach (mehr oder weniger) für die Echtheit dieser Schlüssel, wenn jemand diese überprüft haben möchte. Mit Public-Key-Infrastruktur (PKI) bezeichnet man in der Kryptologie ein System, das digitale Zertifikate ausstellen, verteilen und prüfen kann. Die innerhalb einer PKI ausgestellten Zertifikate werden zur Absicherung rechnergestützter Kommunikation verwendet.

### Aufgabe 3
Was bedeutet Certification-Authority (CA) und was Trust-Center (TC)?

Eine Certification Authority (CA) ist eine vertrauenswürdige Organisation, die digitale Zertifikate ausstellt und verwaltet. Eine CA bestätigt die Identität von Teilnehmern in einem Netzwerk und stellt sicher, dass die von ihnen verwendeten Public-Keys authentisch sind. Die CA verwendet kryptografische Verfahren, um digitale Zertifikate zu erzeugen, die Informationen über den Inhaber des Zertifikats enthalten und von der CA signiert sind. Durch die Signatur der CA können andere Teilnehmer die Echtheit des Zertifikats überprüfen und somit das Vertrauen in den Public-Key des Inhabers aufbauen.

Ein Trust-Center (TC) ist ähnlich wie eine Certification Authority (CA) eine Organisation, die für die Ausstellung und Verwaltung von digitalen Zertifikaten verantwortlich ist. Der Begriff "Trust-Center" wird jedoch manchmal auch verwendet, um ein spezielles Sicherheitssystem oder eine Infrastruktur zu beschreiben, die darauf abzielt, das Vertrauen in digitale Kommunikation und Transaktionen zu gewährleisten. Ein Trust-Center kann verschiedene Aufgaben übernehmen, wie die Verwaltung von Zertifikaten, die Überprüfung von Identitäten, die Bereitstellung von Schlüsselmaterial und die Durchführung von Sicherheitsaudits.

Im Allgemeinen dienen sowohl Certification Authorities als auch Trust-Center dem Zweck, das Vertrauen in die Sicherheit und Echtheit von digitalen Identitäten, Kommunikation und Transaktionen sicherzustellen. Sie spielen eine wichtige Rolle in der Kryptografie und der sicheren Kommunikation im Internet.

### Aufgabe 4
Wer hat das Zertifikat für die Bankwebseite www.ubs.com ausgestellt und wie lange ist es gültig?

**DigiCert Inc**
**Ausgestellt am	Donnerstag, 16. November 2023 um 01:00:00
Gültig bis	Freitag, 13. Dezember 2024 um 00:59:59**

### Aufgabe 5
Wer hat das Zertifikat für die für die Schulwebseite www.tbz.ch ausgestellt und wie lange ist es gültig?

**Let's Encrypt
Ausgestellt am	Montag, 1. April 2024 um 19:35:25
Gültig bis	Sonntag, 30. Juni 2024 um 19:35:24**

### Aufgabe 6
Wer hat das Zertifikat für die für die Webseite www.example.ch ausgestellt und wie lange ist es gültig?

**Diese Website besitzt kein Zertifikat.**

**Da diese Verbindung nicht sicher ist, werden Informationen (z. b. Kenn Wörter oder Kredit Karten) nicht sicher an diese Website gesendet und können von anderen Benutzern abgefangen oder angezeigt werden.**

### Aufgabe 7
Wählen sie irgendeine Applikation aus, die auf ihrem PC installiert ist. Stellen sie sich nun vor, sie müssten diese von Hand aktualisieren oder aus Kompatibilitätsgründen auf eine frühere Version zurückstufen. Wo finden sie aktuelle und frühere Versionen ihrer Software und wie wird sichergestellt, dass die dort angebotene SW-Version auch wirklich echt ist bzw. vom SW-Entwickler stammt?

**TO BE CONTINUE**

### Aufgabe 8
Erstellen sie eine virtuelle Linux-Maschine mit z.B. VirtualBox und Ubuntu. Richten sie nun auf ihrem WIN-PC eine Remoteverbindung via ssh zu ihrem Linux-PC ein. Überprüfen sie die Verbindung. Wäre auch eine graphische Anbindung möglich?

Um eine Remoteverbindung zu einer virtuellen Linux-Maschine über SSH von einem Windows-PC aus einzurichten, sind die folgenden Schritte erforderlich:

1. Richte eine virtuelle Maschine mit Ubuntu als Gastbetriebssystem in VirtualBox ein.
2. Konfiguriere die Netzwerkeinstellungen der virtuellen Maschine (Bridged-Verbindung oder NAT mit Portweiterleitung).
3. Installiere den SSH-Server auf dem Linux-PC in der virtuellen Maschine.
4. Verwende einen SSH-Client wie PuTTY auf dem Windows-PC, um eine SSH-Verbindung zur virtuellen Maschine herzustellen.
5. Gib die IP-Adresse oder den Hostnamen der virtuellen Maschine und den SSH-Port ein.
6. Melde dich mit Benutzername und Passwort in der virtuellen Maschine an, um die Verbindung herzustellen.

Für eine grafische Verbindung gibt es zusätzliche Optionen wie X2Go oder das Remote Desktop Protocol (RDP), die eine grafische Anbindung ermöglichen. Beachte jedoch, dass dies höhere Bandbreite und Konfiguration erfordern kann.

Beachte, dass die genauen Schritte von den spezifischen Versionen der Software abhängen und es sinnvoll ist, die entsprechende Dokumentation zu konsultieren.

### Aufgabe 9
In dieser Übung untersuchen wir eine http-Verbindung und eine https-Verbindung mit dem Network-Sniffer Wireshark:

- https://www.wireshark.org/
- http://www.example.ch
- https://www.zkb.ch
 
Untersuchen sie speziell die OSI-Layer 2,3,4 und 7. Was stellen sie fest? Wo liegen die Unterschiede zwischen http und https? Zusatzfrage: Kann man mit Wireshark bei einer https-Verbindung trotzdem herausfinden, welche Webseite besucht wurde?

Zusammenfassend lässt sich sagen:

- Das OSI-Referenzmodell beschreibt die verschiedenen Schichten, die bei der Netzwerkkommunikation eine Rolle spielen.
- Layer 2 (Data Link) ermöglicht die Übertragung von Datenrahmen zwischen benachbarten Netzwerkknoten.
- Layer 3 (Network) ist für die Adressierung und Weiterleitung von Datenpaketen zwischen verschiedenen Netzwerken zuständig.
- Layer 4 (Transport) bietet Funktionen für Zuverlässigkeit und Fehlerbehebung bei der Datenübertragung.
- Layer 7 (Application) enthält Anwendungsprotokolle wie HTTP und HTTPS für die Kommunikation zwischen Anwendungen.

Der Hauptunterschied zwischen HTTP und HTTPS besteht darin, dass HTTPS eine zusätzliche Sicherheitsschicht verwendet, um die Kommunikation zu verschlüsseln und die Vertraulichkeit und Integrität der Daten zu gewährleisten.

Bei einer HTTPS-Verbindung kann man mit Wireshark den verschlüsselten Datenverkehr sehen, jedoch nicht den Inhalt der übertragenen Daten. Man kann Metadaten wie IP-Adressen und DNS-Anfragen sehen, die Hinweise auf die besuchten Webseiten geben könnten. Um den genauen Inhalt der HTTPS-Verbindung zu sehen, müsste man über den privaten Schlüssel des Servers oder andere Entschlüsselungsmethoden verfügen, was normalerweise nicht der Fall ist.

### Aufgabe 10
Öffnen sie die beiden folgenden Webseiten und achten sie auf die Unterschiede in der Webadresszeile. Was stellen sie bezüglich Protokoll und Zertifikat fest?
- https://juergarnold.ch
- https://www.zkb.ch

**TO BE CONTINUE**

### Aufgabe 11
Wenn sie sich mit Zertifikaten befassen, fallen ihnen früher oder später folgende Anbieter bzw. Webseiten auf:

- http://www.cacert.org
- https://letsencrypt.org/de
 
Was genau wird hier zu welchen Konditionen angeboten?

CAcert.org und Let's Encrypt sind zwei verschiedene Zertifizierungsstellen, die kostenlose SSL/TLS-Zertifikate anbieten.

Bei CAcert.org handelt es sich um eine von der Community betriebene Zertifizierungsstelle. Sie stellt kostenlose Zertifikate aus, die für die digitale Signierung und Verschlüsselung von E-Mails, die Authentifizierung von Benutzern auf Websites und die sichere Datenübertragung im Internet verwendet werden können. Um ein kostenloses Zertifikat von CAcert zu erhalten, kann man sich der CAcert-Community anschließen.

Let's Encrypt ist ebenfalls eine gemeinnützige Zertifizierungsstelle, die kostenlos SSL/TLS-Zertifikate anbietet. Diese Zertifikate werden hauptsächlich für die HTTPS-Verschlüsselung von Websites verwendet, um die Sicherheit und Vertraulichkeit der Internetkommunikation zu gewährleisten.

Beide Zertifizierungsstellen haben unterschiedliche Technologien, Zertifikatsrichtlinien und Verifizierungsprozesse. Es ist wichtig, die spezifischen Anforderungen und Bedingungen jeder Zertifizierungsstelle zu prüfen, um die richtige Wahl entsprechend den individuellen Anforderungen zu treffen.

### Aufgabe 12
Folgende TLS Zertifikatsarten werden unterschieden:
Domain Validated, Organization Validated und Extended Validation. Sie möchten einen Webshop betreiben, wo mit Kreditkarte bezahlt werden kann. Welcher Zertifikatstyp ist der richtige?

Für einen Webshop, in dem Kreditkartenzahlungen akzeptiert werden, wird empfohlen, ein Extended Validation (EV) TLS-Zertifikat zu verwenden. EV-Zertifikate bieten das höchste Maß an Vertrauen und Sicherheit, da eine gründliche Überprüfung der Identität und Rechtsprechung des Unternehmens durchgeführt wird. Mit einem EV-Zertifikat wird der Name des Unternehmens in der Adressleiste des Browsers angezeigt, zusammen mit einem grünen Schlosssymbol, um den Besuchern zu signalisieren, dass es sich um eine vertrauenswürdige Website handelt. Dies hilft, das Vertrauen der Kunden zu stärken und ihnen Sicherheit beim Einkaufen und bei der Eingabe sensibler Informationen wie Kreditkartendaten zu geben. Domain Validated (DV) und Organization Validated (OV) Zertifikate bieten ebenfalls Verschlüsselung, sind aber nicht so stark mit der Identität des Unternehmens verknüpft wie EV-Zertifikate. Daher ist ein EV-Zertifikat die beste Wahl, um das Sicherheitsniveau zu erhöhen und das Vertrauen der Kunden zu gewinnen.

### Aufgabe 13
Studieren sie den Beitrag auf der Webseite Let's Encrypt "Wie es funktioniert"

- https://letsencrypt.org/de/how-it-works/

Was ist der Unterschied zwischen OpenPGP und X.509? 

OpenPGP und X.509 sind Standards für die Verwendung von Public-Key-Kryptographie, haben jedoch unterschiedliche Zwecke und Anwendungsbereiche. 

OpenPGP wird hauptsächlich für die Verschlüsselung und digitale Signatur von E-Mails verwendet. Es ermöglicht sichere Kommunikation zwischen individuellen Benutzern und schützt die Privatsphäre. OpenPGP verwendet eine hierarchische Struktur von Schlüsselpaaren und ermöglicht eine dezentrale Vertrauensbildung.

X.509 wird für die Verwaltung von Zertifikaten in einer Public-Key-Infrastruktur (PKI) verwendet. Es ermöglicht die Authentifizierung von Benutzern, Geräten und Diensten in verschiedenen Anwendungen wie Webbrowsern und VPNs. X.509 verwendet eine zentrale Zertifizierungsstellenstruktur und ein hierarchisches Vertrauensmodell.

OpenPGP-Zertifikate enthalten Informationen über den Schlüsselinhaber, während X.509-Zertifikate zusätzliche Identitätsinformationen wie den Aussteller und Gültigkeitsdaten enthalten. OpenPGP basiert auf persönlichen Vertrauensentscheidungen, während X.509 auf dem Vertrauen in vertrauenswürdige Zertifizierungsstellen beruht.

OpenPGP wird häufig von Einzelpersonen und kleinen Gruppen verwendet, um E-Mails zu sichern. X.509 findet breitere Anwendung in SSL/TLS-Verschlüsselung, Benutzerauthentifizierung und Code-Signierung.

Insgesamt sind OpenPGP und X.509 unterschiedliche Standards mit jeweils spezifischen Einsatzgebieten und Vertrauensmodellen.