# Betriebssysteme

## Was ist ein Betriebssystem?
Damit Anwendungsprogramme auf Computern laufen können, ist ein Betriebssystem erforderlich. Im Einzelnen erfüllen 
Betriebssysteme vor allem die folgenden Aufgaben:
<list>
    <li>
        <strong>Prozessmanagement.</strong> Die Ressourcen des Computersystems müssen zwischen den verschiedenen 
        laufenden Programmen und Systemaufgaben verteilt werden. Zu diesem Zweck werden die einzelnen Aufgaben als 
        sogenannte Prozesse ausgeführt, die vom Betriebssystem als übergeordnetem Steuerprozess verwaltet werden.
    </li>
    <li>
        <strong>Speichermanagement.</strong> Das Speichermanagement sorgt dafür, dass immer die gerade benötigten 
        Speicherinhalte zur Verfügung stehen, ohne dass die Programmierer der Anwendungssoftware sich sonderlich darum 
        kümmern müssten.
    </li>
    <li>
        <strong>Steuerung und Abstraktion der Hardware.</strong> Computersysteme sind hochgradig modular aufgebaut; jede 
        Aufgabe kann durch viele verschiedene Geräte unterschiedlicher Hersteller erledigt werden. Betriebssysteme lösen 
        dieses Problem durch den Einsatz der sogenannten Gerätetreiber, die die Steuerlogik für bestimmte Hardware 
        enthalten. Vor dem Programmierer werden die konkreten Einzelheiten bestimmter Geräte verborgen, weil es 
        vollkommen unzumutbar wäre, beim Schreiben eines Anwendungsprogramms auf die Besonderheiten Hunderter möglicher 
        Geräte einzugehen.
    </li>
    <li>
        <strong>Ein- und Ausgabesteuerung.</strong> Betriebssysteme steuern die Zusammenarbeit mit vielen verschiedenen 
        Ein- und Ausgabekanälen wie Tastatur und Bildschirm, Datenträgern oder Netzwerken.
    </li>
    <li>
        <strong>Dateiverwaltung.</strong> Die Logik der Dateiverwaltung wird in Form sogenannter Dateisysteme vom 
        Betriebssystem zur Verfügung gestellt, damit alle Programme auf dieselbe Art und Weise darauf zugreifen.
    </li>
    <li>
        <strong>Bereitstellen der Benutzeroberfläche.</strong> Das Betriebssystem selbst und alle Programme müssen mit 
        dem Benutzer kommunizieren, um nach dessen Wünschen Aufgaben zu erledigen. Es existieren zwei Arten von 
        Benutzeroberflächen:
        <list>
            <li>
                Die Konsole ermöglicht das dialogbasierte Arbeiten; Benutzer geben per Tastatur Befehle ein und erhalten 
                Antworten.
            </li>
            <li>
                Die grafische Benutzeroberfläche ermöglicht dagegen die intuitive Erledigung von Aufgaben über das 
                Aktivieren von Schaltflächen, Menüs und Symbolen mit der Maus.
            </li>
        </list>
    </li>
</list>

## Entwicklung der Betriebssysteme
Die allerersten Computersysteme der 40er- und 50er-Jahre des letzten Jahrhunderts wurden über Schalter und 
Steckverbindungen programmiert. Dem einzigen Programm, das zu einer bestimmten Zeit auf dem Computer lief, standen 
sämtliche Ressourcen ungeteilt zur Verfügung. Diese Ressourcen waren den Programmierern unmittelbar bekannt, es musste 
keine Abstraktion der Hardwareressourcen stattfinden. Solche Rechner besaßen überhaupt kein Betriebssystem.

Als die Lochkarten Einzug in die Rechenzentren hielten, war es üblich, dass ein Programmierer dem Operator den mithilfe 
eines mechanischen Geräts gestanzten Kartenstapel übergab. Die Programmierer selbst bekamen den eigentlichen Computer 
möglicherweise nicht einmal zu Gesicht, weil nur die mit weißen Kitteln bekleideten Operatoren das »Allerheiligste« 
betreten durften. Der Operator war dafür verantwortlich, den Inhalt des Lochkartenstapels in den Computer einzulesen, 
und händigte dem Programmierer einen Stapel Endlospapier mit den Ergebnissen aus, falls das Programm keine Fehler 
enthielt.

Erst in den 60er-Jahren wurden bestimmte häufig verwendete Programmteile oder Hilfsmittel wie Interpreter für höhere 
Programmiersprachen auf Magnetbändern statt auf Lochkarten abgespeichert. In der ersten Zeit waren wieder die Operatoren 
dafür zuständig, das richtige Band einzulesen, um die Programmlochkarten eines bestimmten Programmierers korrekt zu 
verarbeiten.

Allmählich wurden übergeordnete Steuerprogramme eingeführt, die in der Lage waren, auf Lochkarten mit speziellen 
Metabefehlen zu reagieren, die nicht zum Programm selbst gehörten, sondern organisatorische Informationen enthielten. 
Auf diese Weise konnten einige der Aufgaben von Operatoren automatisiert werden, sodass die Steuerprogramme als 
Operating Systems bezeichnet wurden – noch heute das englische Wort für Betriebssystem. Diese allerersten Systeme 
ermöglichten die automatisierte Abarbeitung mehrerer Lochkartenstapel; diese Form der Verarbeitung wird deshalb als 
Stapelverarbeitung (Batch-Processing) bezeichnet. Dieses Verfahren kommt auch heute noch zum Einsatz, obwohl es sich 
längst nicht mehr um einen Stapel von Lochkarten, sondern um einen Stapel von Befehlen handelt.

»Richtige« Betriebssysteme, wie sie bis heute verwendet werden, wurden allerdings erst eingeführt, als die 
Dialogverarbeitung entwickelt wurde. Seit Mitte der 60er-Jahre wurden immer mehr Rechenzentren mit Terminals 
ausgestattet. Ein Terminal (wegen seiner fehlenden eigenen Rechenfähigkeiten auch »dummes Terminal« – dumb terminal – 
genannt) ist eine Ein- und Ausgabeeinheit, die direkt am Arbeitsplatz eines Programmierers steht und mit dem 
eigentlichen Computer verbunden ist.

Das Betriebssystem muss die Eingabe des Benutzers in den Computer transportieren und die Antwort des Computers an das 
Terminal zurückmelden. Die besondere Herausforderung für die Entwickler der frühen Betriebssysteme bestand darin, die 
Benutzer mehrerer Terminals zeitgleich zu bedienen. Die damaligen Computersysteme waren nämlich erheblich zu selten und 
zu teuer, um einem einzelnen Benutzer sämtliche Ressourcen zu überlassen.

Aus dieser Anforderung entwickelte sich das sogenannte Timesharing-Verfahren, das die Anfragen mehrerer Benutzer 
scheinbar gleichzeitig verarbeitet, indem es die Rechenzeit in kleine Einheiten (Zeitscheiben, Time Slices) unterteilt 
und den Anforderungen der einzelnen Benutzer der Reihe nach zuweist. Aus diesem grundsätzlichen Prinzip entwickelte sich 
beispielsweise das moderne Multitasking, das die Ausführung mehrerer Programme auf demselben Rechner ermöglicht. 
Außerdem wurden allmählich Mechanismen eingeführt, um die Arbeit verschiedener Benutzer im Speicher des Rechners 
voneinander zu trennen. Die Grundlagen der Zugriffsrechte, der persönlichen Anmeldung und des Speicher- und 
Ressourcenmanagements wurden damit entwickelt.

Die ersten Timesharing-Betriebssysteme wurden für einzelne Computer und ihre Anwender in Universitäten und anderen 
großen Institutionen hergestellt. Eines der wenigen frühen Beispiele, die relativ bekannt geworden sind, ist das am MIT 
(Massachusetts Institute of Technology) entwickelte ITS (Incompatible Timesharing System) – es wurde von Richard M. 
Stallman mitentwickelt, dem Begründer der Idee der freien Software. Einige der Fähigkeiten von ITS wurden später in Unix 
aufgenommen.

Der erste Versuch, ein kommerzielles Timesharing-System zu schreiben, erfolgte Ende der 60er-Jahre: Die Bell 
Laboratories, das Entwicklungszentrum der US-Telefongesellschaft AT&T, arbeiteten mit einigen anderen Firmen an einem 
System namens MULTICS. Die Idee war, viele Hundert Terminals an einem für damalige Verhältnisse recht mächtigen Rechner 
anzuschließen. Leider wurde MULTICS erst viel später fertiggestellt, als es kaum noch jemanden interessierte.

### Die Geschichte von Unix
Einige Ideen von MULTICS inspirierten jedoch Ken Thompson von den Bell Labs dazu, mit der Arbeit an einem eigenen 
Betriebssystem zu beginnen. Anfangs war es als Einzelplatzsystem geplant und wurde auf einem PDP-7-Kleincomputer von 
Digital Equipment (DEC) entwickelt, der, verglichen mit der für MULTICS verwendeten Maschine, nicht besonders 
leistungsfähig war. Thompson und sein späterer Mitstreiter Dennis Ritchie nannten ihr Betriebssystem in einer Anspielung 
auf MULTICS Unics; nach einiger Zeit wurde daraus Unix. Die ursprünglich nicht geplante Mehrbenutzerfähigkeit wurde 
übrigens sehr schnell nachgerüstet, nachdem die ersten Versionen von Unix gut funktionierten.

Eines der wichtigsten Designmerkmale des Betriebssystems Unix ist seine Modularität: Jeder (als eigenständiges Programm 
realisierte) Befehl und jeder Bestandteil des Systems kann einzeln ausgetauscht werden, ohne das Gesamtsystem ändern zu 
müssen. Unix wurde zunächst in der Maschinensprache der PDP-7 programmiert. Ab 1971 entwickelten Dennis Ritchie und 
Brian Kernighan dann die Programmiersprache C, in der Unix schließlich neu geschrieben wurde. Da C-Compiler bald für 
verschiedene Computersysteme verfügbar waren, fand Unix schnell Verbreitung.

Eine kommerzielle Verbreitung von Unix war anfangs nicht möglich. Da AT&T in den 70er-Jahren noch das 
US-Telekommunikationsmonopol innehatte, durfte das Unternehmen keine Geschäfte in anderen Branchen wie etwa dem 
Computerbereich tätigen. Deshalb wurden Lizenzen für den Unix-Quellcode unter sehr lockeren Bedingungen an Universitäten 
vergeben. Das ist der Grund, warum die Grundlagen des Betriebssystemaufbaus bis heute vornehmlich am Beispiel von Unix 
und seinen Nachfolgesystemen gelehrt werden.

Die aktivste aller Universitäten, die den Unix-Quellcode erhielten, war die University of California in Berkeley. Die 
dortigen Programmierer erweiterten das ursprüngliche Unix und brachten schließlich eine eigene Version heraus, die 
Berkeley System Distribution (BSD). Als AT&T schließlich in den 80er-Jahren die Lizenz erhielt, Unix kommerziell zu 
vertreiben, hatten sich die AT&T-Version, genannt System V, und die BSD bereits erheblich auseinanderentwickelt. Zudem 
wurde die Berkeley University verpflichtet, sämtliche Bestandteile des AT&T-Unix aus der BSD zu entfernen.

Seitdem ist jede kommerzielle und jede freie Unix-Version eine mehr oder weniger starke Mischung aus BSD- und 
System-V-Features. Allerdings haben System V und BSD wieder zahlreiche Fähigkeiten voneinander übernommen, sodass es 
nicht immer ganz leicht ist, sie auseinanderzuhalten.

Heute existiert eine Vielzahl unterschiedlicher Unix-kompatibler Betriebssysteme. Dazu gehören oder gehörten 
kommerzielle Systeme wie Sun Solaris, IBM AIX, HP UX und freie Varianten wie etwa Linux oder FreeBSD. Eine 
Sonderstellung nimmt Apples Betriebssystem macOS (vormals Mac OS X, zwischenzeitlich nur OS X) ein: Es basiert auf einer 
Version der BSD, der Betriebssystemkern Darwin ist Open-Source-Software und läuft auf verschiedenen Plattformen. Die 
grafische Benutzeroberfläche Aqua ist dagegen eine kommerzielle Eigenproduktion von Apple und funktioniert nur auf Macs 
mit PowerPC-, Intel-Prozessoren oder den Hauseigenen ARM-Prozessoren.

Die Mindestanforderung dessen, was ein Unix-System leisten muss, ist in einem Standard namens POSIX (Portable Operating 
System Interface)festgeschrieben. Allerdings werden von einem »richtigen« Unix heute auch einige weitere Quasi-standards 
verlangt, die nicht im POSIX-Standard festgelegt sind. Am wichtigsten ist dieser Standard für Programmierer. Möchte man 
als Programmierer ein Programm POSIX-konform schreiben, kann davon ausgegangen werden, dass es sich unter jeder 
beliebigen Unix-Version kompilieren lässt.

Anfang der 90er-Jahre sah es übrigens bereits fast so aus, als würde Unix nicht mehr lange überleben: Die verschiedenen 
Varianten entwickelten sich zunehmend auseinander. Auf dem Desktop dominierte Microsoft Windows, während Server für die 
immer häufiger eingesetzten PC-Netzwerke vor allem unter Novell NetWare betrieben wurden.

Zwei wichtige Umstände haben Unix gerettet und machen es heute, über 40 Jahre nach seiner Entwicklung, zu einem der 
gefragtesten Betriebssystemkonzepte: Der eine Grund ist die immense Ausbreitung des Internets, dessen wichtigste 
Konzepte unter Unix entwickelt wurden. Der zweite Anlass für die Verbreitung von Unix ist die Erfolgsgeschichte des 
freien Betriebssystems Linux, das 1991 von dem finnischen Informatikstudenten Linus Torvalds entwickelt wurde und 
inzwischen das Betriebssystem mit dem größten jährlichen Wachstum ist.


### PC-Betriebssysteme
Eine völlig andere Entwicklungslinie im Bereich der Betriebssysteme begann mit der Entwicklung der Personal Computer ab 
Mitte der 70er-Jahre. Auf das Timesharing und den Mehrbenutzerbetrieb wurde bei den ersten Versionen von 
PC-Betriebssystemen zugunsten der Performance-steigerung zunächst völlig verzichtet.

Der erste weitverbreitete PC war der von Steve Wozniak und Steve Jobs 1977 entwickelte Apple II. Er erlaubte es, an 
einer wenig komfortablen Konsole BASIC- und Systembefehle einzutippen. Wurde einem Befehl eine Zeilennummer 
vorangestellt, dann wurde er Teil eines im Arbeitsspeicher abgelegten Programms, das beispielsweise mithilfe von RUN 
gestartet und über LIST auf dem Bildschirm angezeigt werden konnte. Befehle ohne Zeilennummer wurden dagegen unmittelbar 
ausgeführt.

Dieses Konzept wurde in den 80er-Jahren von unzähligen Homecomputern wie dem Commodore C64, dem Atari 800XL oder dem 
Sinclair ZX81 und ZX Spectrum nachgeahmt. Diese in das ROM eingebauten BASIC-Editoren und -Interpreter lassen sich 
allerdings nicht als vollwertige Betriebssysteme bezeichnen.

Das erste »richtige« Betriebssystem für Personal Computer wurde von Gary Kildall entwickelt. Es hieß CP/M (Control 
Program for Microcomputers). Im Vergleich zu den bereits weit fortgeschrittenen Betriebssystemen für Großrechner und 
Kleincomputer war es ziemlich primitiv, hatte aber mehrere Vorteile: Es lief auf zwei verschiedenen, zu jener Zeit 
weitverbreiteten Prozessorplattformen, dem Intel 8080 und dem Zilog Z80. Außerdem besaß es eine Dateiverwaltungsfunktion 
für Diskettenlaufwerke und konnte über verschiedene Konsolenbefehle gesteuert werden.

#### DOS und Windows

#### Linux

## Aufgaben und Konzepte

### Zusammengefasst: allgemeiner Aufbau von Betriebssystemen

#### Der Kernel

#### Gerätetreiber

#### Systemprogramme

#### Die Schnittstelle für

#### Anwendungsprogramme

#### Die Benutzeroberfläche

### Prozessverwaltung

#### Das Unix-Prozessmodell

#### Deadlocks

#### Threads

### Speicherverwaltung

### Dateisysteme

#### Das virtuelle Unix-Dateisystem

#### Das virtuelle Windows-Dateisystem