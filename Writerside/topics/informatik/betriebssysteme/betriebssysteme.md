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
1981 kam dann der IBM-PC auf den Markt, der bald zum erfolgreichsten Personal Computer wurde. IBM wollte ein 
CP/M-ähnliches Betriebssystem für diesen Rechner haben. Gary Kildall war jedoch nicht bereit, IBMs 
Verschwiegenheitserklärungen zu unterschreiben. Deshalb wandte sich IBM an die junge Firma Microsoft, die in Seattle 
arbeitete und Programmiersprachen-Pakete für verschiedene PCs produzierte. Bill Gates, der die Firma 1975 mit seinem 
Schulfreund Paul Allen gegründet hatte, fand bei einem Unternehmen namens Seattle Computer Products einen halb fertigen 
CP/M-Nachbau namens QDOS – Quick and Dirty Operating System. Angeblich kaufte Bill Gates alle Rechte an diesem System 
für 50.000 US$. Microsoft verbesserte das System und lieferte es als MS-DOS (Microsoft Disk Operating System) an IBM. 
Eine leicht modifizierte Fassung wurde unter dem Namen IBM PC DOS mit jedem IBM-PC ausgeliefert. Die meisten später 
erschienenen kompatiblen Geräte enthielten dann ab Werk das eigentliche MS-DOS. Auf diese Weise entstand das bis heute 
andauernde Kerngeschäft von Microsoft, denn weltweit wird noch immer fast jeder neue PC mit einem 
Microsoft-Betriebssystem ausgeliefert.

CP/M, MS-DOS und einige andere Versuche besaßen allesamt nur eine Konsole, keine grafische Benutzeroberfläche. Dabei war 
diese bereits ab 1963 als Designstudie von Douglas Engelbart entwickelt worden. Im Forschungszentrum Xerox PARC wurde 
sie etwa Mitte der 70er-Jahre fertiggestellt. Allerdings waren die Manager von Xerox nicht in der Lage, die 
Entwicklungen der PARC-Forscher zu verstehen und zur Marktreife zu bringen. Erst Anfang der 80er-Jahre besichtigte Steve 
Jobs von Apple das PARC und verliebte sich auf den ersten Blick in die grafische Oberfläche. Daraufhin erschien im Jahr 
1983 der teure Flop Apple Lisa; 1984 kam schließlich der Macintosh auf den Markt. Beide waren mit Maus und grafischer 
Oberfläche ausgestattet.

Auf den IBM-PCs hielt die grafische Benutzeroberfläche erst Jahre später Einzug. Da der Macintosh einen gewissen, wenn 
auch anfangs noch keinen überwältigenden Erfolg hatte, beschloss Bill Gates, dass auch der PC ein Graphical User 
Interface (GUI) erhalten sollte. 1990 erschien schließlich die erste brauchbare Version von Microsoft Windows; zunächst 
als grafischer Aufsatz für MS-DOS.

Ebenfalls im Jahr 1990 wurde der Prozessor Intel 80386 eingeführt. Es handelte sich um den ersten 32-Bit-Prozessor der 
Intel-Baureihe. Der IBM PC/AT und kompatible Geräte anderer Hersteller wurden bald damit ausgestattet. Ärgerlicherweise 
war MS-DOS jedoch ein reines 16-Bit-Betriebssystem, das bestimmte eingebaute Fähigkeiten des 386er wie Speicherschutz, 
Multitasking und die Adressierung von mehr Arbeitsspeicher nicht nutzen konnte.

In dieser Situation wurde bei IBM ein neues Betriebssystem konzipiert. Das 32-Bit-System OS/2 sollte zusammen mit dem 
neuartigen PC-System PS/2 verkauft werden. Dieses Computersystem sollte durch patentierte, inkompatible Schnittstellen 
die Hersteller IBM-kompatibler PCs ausbooten. Die Programmierung von OS/2 wurde zunächst in Zusammenarbeit mit Microsoft 
in Angriff genommen. Schließlich gerieten die beiden Firmen jedoch in Streit, weil IBM Windows nicht unterstützen wollte 
und voll auf OS/2 setzte. Letztlich setzte sich Windows als wichtigstes PC-Betriebssystem durch. Dennoch besaß OS/2, 
dessen bisher letzte Version Warp 4 im Jahr 1996 erschien, einige hervorragende Konzepte.

Microsoft blieb dagegen noch jahrelang bei DOS als Betriebssystem und Windows als grafischer Erweiterung, wobei DOS 
jedoch allmählich zum Windows-Starter verkam und Windows – zumindest teilweise – mit 32-Bit-Fähigkeiten ausgestattet 
wurde. Parallel entwickelte Microsoft ein völlig neues Betriebssystem namens Windows NT (New Technology). Als 
Chefentwickler konnte Microsoft David Cutler gewinnen, der das Betriebssystem VMS für die legendären VAX-Rechner von 
DEC entwickelt hatte. 1993 erschien die erste Version, die aufgrund der Windows-3.0-Benutzeroberfläche als Windows NT 
3.0 bezeichnet wurde.

1995 kam Windows 95 auf den Markt, die Privatkunden-Version eines 32-Bit-Windows-Systems mit modernisierter, stärker von 
Mac OS beeinflusster grafischer Oberfläche. Unter der Oberfläche war es noch immer ein DOS-Betriebssystem, das die 
Windows-Umgebung startete. Allerdings waren die meisten 32-Bit-Errungenschaften nun auch in Windows 95 verfügbar, 
beispielsweise auch die sehnsüchtig erwarteten langen Dateinamen. 1996 wurde Windows NT 4.0 vorgestellt, das die neue 
Oberfläche von Windows 95 auch in der NT-Welt einführte.

Erst das 2001 eingeführte Windows XP brachte schließlich auch in der Privatkunden-Welt den Umstieg auf NT-Technologie. 
Das System wurde in einer Home- und einer Professional-Version angeboten.

Zuvor waren noch zwei Nachfolger von Windows 95 namens Windows 98 und Windows Me (Millennium Edition) erschienen; das 
ursprünglich Windows NT 5.0 genannte System kam 1999 als Windows 2000 auf den Markt.

Anfang 2007 stellte Microsoft mit Windows Vista endlich den seit Langem entwickelten XP-Nachfolger bereit. Das System 
wurde in sieben verschiedenen Versionen verkauft, vom minimalen Vista Home Basic über mehrere Home- und 
Business-Varianten bis hin zum voll ausgestatteten Vista Ultimate.

Im Oktober 2009 erschien Windows 7, und 2012 wurde Windows 8 vorgestellt – beide ebenfalls in verschiedenen Editionen. 
In Windows 8 wurde erstmals versucht, eine einheitliche Bedienoberfläche für PCs, Tablets und Smartphones zu etablieren; 
unter anderem wurde der Desktop durch ein erweitertes Startmenü mit konfigurierbaren rechteckigen Kacheln ersetzt. Viele 
Benutzer hielten diesen ersten Versuch für nicht sonderlich gelungen, sodass das bald darauf erschienene Windows 8.1 
einige der Änderungen wieder rückgängig machte: Genau wie bei Windows 10 wird hier nach dem Start erst einmal wieder der 
klassische Desktop angezeigt, und eine durch die Windows-8-Kacheln erweiterte Version des Startmenüs erscheint erst nach 
Klick auf die Start-Schaltfläche.

#### Linux
Der 386er-PC brachte nicht nur der Windows-Familie den Durchbruch, sondern war auch der Anlass für Linus Torvalds, das 
Betriebssystem Linux zu entwickeln. Er war ein wenig enttäuscht von den eingeschränkten Möglichkeiten des zu Lehrzwecken 
entwickelten abgespeckten Unix-Systems Minix und wollte auf keinen Fall Windows benutzen. Aus diesem Grund begann er mit 
der Entwicklung seines eigenen Systems.

Das Betriebssystem Linux ist ein voll ausgestattetes POSIX-konformes Unix-Betriebssystem, dessen Kernel allerdings von 
seinem Erfinder Linus Torvalds vollkommen neu entwickelt wurde. Seit seiner ursprünglichen Entwicklung im Jahr 1991 
wurde der Linux-Kernel durch die Mitarbeit zahlloser Freiwilliger immer weiter ausgebaut. Heute unterstützt er beinahe 
jede erdenkliche Hardware und läuft nicht etwa nur auf der Intel-PC-Architektur, sondern wurde auf viele verschiedene 
Plattformen portiert, beispielsweise PowerPC, Alpha, Sun SPARC oder diverse IBM-Großrechner. In Form von Google Android 
läuft eine Variante auch auf zahllosen Smartphones und Tablets.

Selbstverständlich besteht ein Unix-System wie Linux aber nicht nur aus dem Kernel. Um damit arbeiten zu können, wird 
eine Benutzeroberfläche in Form einer Shell oder eines grafischen Desktops benötigt (alle aktuellen Linux-Distributionen 
bieten beides). Ein weiterer wichtiger Bestandteil eines Unix-Systems sind die zahlreichen Systemprogramme. Die 
Linux-Versionen dieser Programme sind kompatibel mit den entsprechenden Befehlen kommerzieller Unix-Versionen, 
entstammen aber größtenteils dem GNU-Projekt (<a href="http://www.gnu.org">http://www.gnu.org</a>). Diese Abkürzung 
steht für GNU’s Not Unix; es handelt sich um ein rekursives Akronym, in dem der erste Buchstabe immer wieder für den 
Namen des Ganzen steht – eine beliebte Form der Unterhaltung in der Unix- und Open-Source-Szene. Aus diesem Grund müsste 
ein vollständiges Linux-System aus Kernel und Dienstprogrammen korrekterweise als GNU/Linux bezeichnet werden, aber 
daran hält sich nur die Distribution Debian.

Das GNU-Projekt wurde 1984 von Richard Stallman ins Leben gerufen und setzte sich zum Ziel, freie Versionen sämtlicher 
Unix-Systemprogramme zu entwickeln. Deshalb gründete Stallman gleichzeitig die Free Software Foundation (FSF, 
<a href="http://www.fsf.org">http://www.fsf.org</a>). Als Linus Torvalds mit der Arbeit an Linux begann, existierte 
bereits ein C-Compiler (der GNU C Compiler oder GCC); auch die meisten Standardbefehle waren bereits verfügbar. Die 
meisten GNU-Varianten der Unix-Programme sind inzwischen sogar leistungsfähiger als die ursprünglichen Versionen. 
Lediglich der lange geplante GNU-Kernel Hurd ist bis heute nicht als finale Version erschienen, zumal er durch die 
Entwicklung von Linux im Grunde überflüssig wurde.

Freie Software hat nicht nur etwas damit zu tun, dass die Programme kostenlos erhältlich sind, sondern auch damit, dass 
man den Quellcode erhält und damit fast alles machen darf, was man möchte. Deshalb lautet ein Motto der Free Software 
Foundation »Free software is a matter of liberty, not price« (»Freie Software ist eine Frage der Freiheit, nicht des 
Preises«). Kommerzielle Softwarelizenzen enthalten nämlich in der Regel eine Reihe von Einschränkungen und erlauben im 
Grunde nichts weiter, als die Software für ihren offiziellen Anwendungszweck einzusetzen. Die FSF hat dafür eine eigene 
Softwarelizenz ausgearbeitet, die vor allem verhindern soll, dass kommerzielle Softwareentwickler freie Softwareprojekte 
an sich binden und die ursprüngliche Freiheit beeinträchtigen. Unter dieser Lizenz, der GNU General Public License 
(GPL), wird übrigens auch Linux selbst verbreitet.

Zu Beginn seiner Entstehung war Linux vor allem im Kreis der Entwickler verbreitet, die daran arbeiteten. Es war 
schwierig, den Linux-Kernel zu installieren und die GNU-Versionen aller erforderlichen Systemprogramme zu beschaffen und 
miteinander zu koordinieren. In den ersten Jahren wurde Linux deshalb vornehmlich von Informatikern und interessierten 
Studenten weitergereicht, da die Universitäten bereits über Internetanbindungen verfügten, als der Rest der Welt noch 
nichts damit zu tun hatte.

Einige der Studenten, die mit Linux arbeiteten, begannen allmählich, den Kernel und die Systemprogramme 
zusammenzustellen und Installationsprogramme für diese Betriebssystempakete zu schreiben. Aus diesen ersten Bemühungen 
entstanden allmählich verschiedene Linux-Distributionen, die anfangs auf Disketten, später auf CD-ROMs, noch später auf 
DVDs und in den letzten Jahren vorwiegend als Download verbreitet wurden, oft zusammen mit mehr oder weniger 
ausführlichen gedruckten Dokumentationen. Firmen wurden gegründet, die solche Distributionen erstellten und zu 
vergleichsweise günstigen Preisen verkauften.

Der Kauf einer Distribution hat nichts mit dem Erwerb kommerzieller Software gemeinsam: die Software, die man erhält, 
darf auf beliebig vielen Rechnern installieren und an allen Bekannten weitergegeben werden. Die Distributoren erhalten 
das Geld nicht für die Software selbst oder für ein Nutzungsrecht daran, sondern lediglich für ihre Arbeit an 
Installationsprogrammen und Dokumentationen. Eine Distribution kann allerdings einzelne kommerzielle Programme 
enthalten, für die andere Bedingungen gelten. Hierbei ist die Beschreibung, die der Distributor mitliefert, zu beachten.

Heute ist eine Reihe verschiedener Distributionen erhältlich, die sich bezüglich ihres Umfangs, ihres 
Anwendungsschwerpunkts und ihres Preises unterscheiden.

## Aufgaben und Konzepte

### Zusammengefasst: allgemeiner Aufbau von Betriebssystemen
Jedes Betriebssystem besitzt gewisse Grundbestandteile, denn alle Systeme müssen Computer verwalten, die bestimmte 
Gemeinsamkeiten aufweisen. Beinahe jedes neuere Betriebssystem besteht aus dem Kernel, den mehr oder weniger fest zu 
diesem gehörenden Gerätetreiber, den Systemprogrammen, einer Schnittstelle für Anwendungsprogramme und einer 
Benutzeroberfläche.

#### Der Kernel
Der Kernel (das englische Wort für Kern, beispielsweise ein Obstkern) ist das grundlegende Computerprogramm, das 
unmittelbar auf dem Prozessor des Rechners ausgeführt wird. Er läuft bis zum Herunterfahren des Systems permanent im 
Hintergrund und steuert alle anderen Betriebssystemkomponenten sowie den Start und den Ablauf der Anwendungsprogramme. 
Der Kernel initialisiert die Zusammenarbeit mit der Hardware, indem er die Treiber lädt und koordiniert. Aus einer 
technischen Perspektive kann man sich vorstellen, dass der Kernel das einzige echte Programm ist, das permanent 
ausgeführt wird, während alle anderen Programme, die später geladen werden, nur Unterprogramme sind, die vom Kernel 
aufgerufen werden und die Kontrolle durch einen Rücksprung wieder abgeben.

Es gibt unterschiedlich konzipierte Kernels. Das ältere Kernel-Konzept ist der sogenannte monolithische Kernel, der so 
viele Funktionen wie möglich selbst ausführt. Moderner ist das Konzept des Mikrokernels, der so wenig wie möglich selbst 
tut und die meisten Aufgaben an Prozesse delegiert, die im Benutzermodus laufen wie gewöhnliche Anwendungsprogramme.

Da Mikrokernels kleine und elegante Programme sind und die einzelnen Teile des Betriebssystems nur bei Bedarf im 
Speicher halten, müssten Betriebssysteme auf Mikrokernel-Basis theoretisch schneller und effizienter laufen als Systeme 
mit monolithischen Kernels. Allerdings wird dabei oft vergessen, dass der ständige Wechsel zwischen Benutzer- und 
Kernel-Modus Zeit und Ressourcen verbraucht. Außerdem können auch monolithische Kernel inzwischen häufig von einem der 
entscheidenden Vorteile des Mikrokernels profitieren: Die meisten Gerätetreiber sind modular, können also je nach Bedarf 
geladen und wieder aus dem Speicher entfernt werden. Dies ist besonders wichtig für hot-plugging-fähige Schnittstellen 
wie USB, FireWire oder Bluetooth.

Ein weiterer Fortschritt ist das Threading-Modell, das in immer mehr Betriebssystemen zum Einsatz kommt. Die 
schwerfälligen Prozesse werden durch eine leichtgewichtige Alternative namens Threads ergänzt, was die Arbeit des 
Kernels weiter beschleunigt.

Anfang der 90er-Jahre schienen die Mikrokernel sich allmählich durchzusetzen, es wurden um diese Zeit kaum noch völlig 
neue Betriebssysteme auf der Basis eines monolithischen Kernels konzipiert. Eine wichtige Ausnahme ist Linux – sein 
Kernel ist bis heute monolithisch, verwendet aber modulare Gerätetreiber und inzwischen auch Threads. Andrew Tanenbaum, 
der Entwickler von Minix und Autor mehrerer brillanter Fachbücher über Betriebssysteme und andere Informatikthemen, 
verfasste aus diesem Grund in der Minix-Newsgroup einen berühmt gewordenen Beitrag mit dem Titel »Linux is obsolete« 
(»Linux ist überholt«). Inzwischen gehört Linux allerdings zu denjenigen Systemen, die in seinem Lehrbuch »Moderne 
Betriebssysteme« als Anschauungsbeispiele dienen.

Ein wichtiges Betriebssystem mit Mikrokernel, und zwar dem bekannten Mach-Mikrokernel, ist macOS. Die meisten anderen 
Unix-Systeme besitzen dagegen wie Linux einen monolithischen Kernel. In gewisser Weise lässt sich der Kernel von Windows 
NT und seinen Nachfolgern auch als Mikrokernel beschreiben.

Wenn ein Computer eingeschaltet wird, führt das BIOS des Rechners zunächst einige Überprüfungen durch und übergibt die 
Kontrolle anschließend dem Bootloader eines Betriebssystems. Der Bootloader ermöglicht entweder die Auswahl mehrerer 
Betriebssysteme, die auf den Datenträgern des Rechners installiert sind, oder startet unmittelbar ein bestimmtes System. 
Das Booten (kurz für Bootstrapping –»die Stiefel schnüren«) eines Betriebssystems bedeutet zunächst, dass der Kernel 
geladen und ausgeführt wird. Dieser erledigt alle weiteren erforderlichen Aufgaben.

Wichtig ist es, die bei den meisten Betriebssystemen (insbesondere Unix und Windows) zu beobachtende Trennung zwischen 
Kernelmodus und Benutzermodus zu verstehen. Ein Prozess, der im Kernelmodus läuft, besitzt gewisse Privilegien, die im 
Benutzermodus nicht vorhanden sind. Bei den meisten Computern werden für die beiden Modi unterschiedliche Betriebsmodi 
des Prozessors selbst verwendet. Beispielsweise besitzen Intel-Prozessoren und damit kompatible Prozessoren seit dem 
386er vier verschiedene Modi, die sich durch einen unterschiedlich starken Schutz vor Interrupts, das heißt 
Unterbrechungsanforderungen durch Hardware oder bestimmte Programmschritte, unterscheiden. Für gewöhnlich wird der Modus 
mit dem stärksten Schutz als Kernelmodus und der mit dem geringsten als Benutzermodus verwendet.

Prozesse im Kernelmodus erledigen wichtige Betriebssystemaufgaben, die nicht durch Prozesse im Benutzermodus 
unterbrochen werden dürfen. Beispielsweise sorgen sie für die eigentliche Verarbeitung von Hardware-Interrupts, das 
Öffnen und Schließen von Dateien oder die Speicherverwaltung. Auch wenn ein Prozess im Kernelmodus nicht von außen 
unterbrochen werden kann, kann er freiwillig die Kontrolle an einen anderen Prozess abgeben. In der Regel ruft er den 
Task Scheduler auf, der ebenfalls im Kernelmodus läuft und für die Verteilung der Rechenzeit an die verschiedenen 
Prozesse zuständig ist.

Ein Prozess im Benutzermodus kann jederzeit unterbrochen werden, etwa durch einen Hardware-Interrupt, durch einen 
aufwachenden Kernelprozess oder dadurch, dass er selbst einen Befehl aufruft, der nur im Kernel-Modus ausgeführt werden 
kann. Letzteres sind die sogenannten Systemaufrufe(System Calls), die es Programmierern ermöglichen, die eingebauten 
Funktionen des Betriebssystems zu nutzen.

Mikrokernel-basierte Betriebssysteme versuchen, so gut wie alle Aufgaben im Benutzermodus auszuführen. Der Kernel selbst 
nimmt im Wesentlichen nur noch die Prozessverwaltung vor; selbst das Speichermanagement und die Ein-/Ausgabekontrolle 
finden im Benutzermodus statt. Auf diese Weise kann ein Mikrokernel-System zwar flexibler auf Anforderungen reagieren, 
muss dafür aber häufiger zwischen Kernel- und Benutzermodus hin- und herschalten, was zusätzliche Performance kostet.

Windows NT und seine Nachfolger (einschließlich Vista, Windows 7, 8 und 10) verwenden einen Mittelweg zwischen 
Mikrokernel-System und monolithischem Kernel-System: Gewisse Teile wurden aus dem Kernel ausgelagert und bilden 
sogenannte Subsysteme, die im Benutzermodus laufen und verschiedene Teilfunktionen anbieten, die kernelartige Aufgaben 
erledigen. Andere Teile des Betriebssystems laufen dagegen im Kernel-Modus.

Es gibt in der Praxis keine Betriebssysteme mehr, die keine richtige Trennung zwischen Kernel- und Benutzermodus 
durchführen. Die letzten waren MS-DOS in Kombination mit Windows 3.11, der letzten Windows-Version, die kein 
vollständiges Betriebssystem war, und Mac OS bis zur Version 9(das aktuelle macOS ist dagegen eine völlige 
Neuentwicklung, die von dem UNIX-System NeXTSTEP abstammt).

Der auffälligste Unterschied zwischen einem modernen System und solchen altmodischen Betriebssystemen besteht darin, 
dass Letztere nur das veraltete kooperative Multitasking verwenden – ein Prozess entscheidet selbst, wann er die 
Kontrolle an das Betriebssystem zurückgeben möchte. Stürzt ein Programm ab, das in einem solchen Prozess läuft, dann 
ist sehr wahrscheinlich das gesamte Betriebssystem instabil geworden. Das in modernen Systemen eingesetzte präemptive 
Multitasking entscheidet dagegen selbst, wie lange Prozesse im Benutzermodus die Rechenzeit behalten dürfen, und 
entzieht ihnen diese bei Bedarf wieder.

Außerdem besitzen veraltete Betriebssysteme kein richtiges Speichermanagement; Prozesse können gegenseitig auf ihre 
Speicherbereiche zugreifen und diese versehentlich überschreiben.

#### Gerätetreiber
Die Gerätetreiber (Device Drivers) sind spezielle kleine Programme, die sich um die Steuerung einzelner 
Hardwarekomponenten kümmern. In manchen Betriebssystemen sind Treiber ein fester Bestandteil des Kernels, während sie in 
den meisten neueren Systemen als Module vorliegen, die sich bei Bedarf laden und wieder aus dem Speicher entfernen 
lassen.

Es ist eine der schwierigsten Aufgaben für Programmierer, Gerätetreiber zu schreiben. Der Treiber bildet die 
Schnittstelle zwischen Betriebssystem und Hardware. Er muss die allgemeinen Anforderungen des Betriebssystems an eine 
bestimmte Geräteklasse in die spezifische Sequenz von Steuerbefehlen umsetzen, die das Gerät eines bestimmten 
Herstellers versteht, und umgekehrt die Antworten des Geräts wieder in eine allgemein verständliche Form bringen.

Aus der Sicht von Treibern lassen sich zwei grundsätzliche Arten von Geräten unterscheiden: Zeichengeräte (Character 
Devices oder kurz Char Devices) tauschen Daten mit ihrer Umgebung als sequenzielle Datenströme aus. Die Daten werden 
also Zeichen für Zeichen nacheinander ausgelesen. Typische Beispiele sind die Tastatur, ein Drucker oder ein 
Bandlaufwerk. Blockgeräte (Block Devices) stellen sich dagegen ähnlich dar wie der Arbeitsspeicher: Der Zugriff auf den 
Inhalt des Geräts kann in beliebiger Reihenfolge blockweise erfolgen. Zu den Blockgeräten zählen vornehmlich die meisten 
Laufwerke wie die Festplatte oder ein CD-ROM-Laufwerk, aber auch zum Beispiel Grafikkarten.

Damit ein Treiber für ein bestimmtes Gerät geschrieben werden kann, muss der Hersteller die Schnittstellen dieses Geräts 
veröffentlichen. Einige Hersteller wollen dies nicht und bieten stattdessen lieber selbst Treiber für die wichtigsten 
Betriebssysteme an. Bevor ein bestimmtes Gerät angeschafft wird, muss also sichergestellt werden, dass ein Treiber fürs 
Betriebssystem verfügbar ist.

#### Systemprogramme
Diejenigen Bestandteile des Betriebssystems, die nicht zum Kernel gehören, liegen in der Regel als unabhängige Programme 
vor, die willkürlich geladen, ausgeführt und wieder beendet werden können. Bei einem Betriebssystem mit 
Konsolen-Oberfläche muss man die Namen dieser Programme kennen, weil sie durch Eingabe ihres Namens aufgerufen werden. 
In einer grafischen Benutzeroberfläche werden sie dagegen hinter den Kulissen automatisch aufgerufen, wenn 
beispielsweise das Symbol des Programms per Doppelklick ausgewählt wird.

Verschiedene Betriebssysteme verfügen über unterschiedlich mächtige Systemprogramme. Unix-Systeme sind mit besonders 
leistungsfähigen Systemprogrammen ausgestattet, weshalb Unix-Benutzer häufiger als die Anwender anderer Betriebssysteme 
die Konsole verwenden, obwohl auch Unix-Systeme inzwischen mit sehr überzeugenden grafischen Oberflächen ausgestattet 
sind.

Bei einem Unix-System kann jede beliebige Verwaltungsaufgabe über die Konsole erledigt werden, während unter Windows 
einige Werkzeuge nur unter der grafischen Oberfläche zur Verfügung stehen. Aus diesem Grund können Unix-Rechner auch von 
fern über ein Netzwerk bedient werden. Die Konsole kann über eine Terminal-Emulation zur Verfügung gestellt werden, ein 
Programm auf einem anderen Rechner übernimmt also die Funktion eines Terminals. Das einzige System, bei dem 
Systemprogramme nicht ohne Weiteres direkt aufgerufen werden konnten, weil es überhaupt keine Konsole besaß, war das 
veraltete Mac OS bis einschließlich Version 9.

Typische Systemprogramme sind beispielsweise Befehle zur Manipulation von Dateien und Verzeichnissen, etwa für das 
Umbenennen, Löschen oder Kopieren. Außerdem gehören allerlei Steuerungs- und Analysewerkzeuge dazu.

Systemprogramme sind übrigens nicht zu verwechseln mit Systemaufrufen. Letztere werden von Prozessen in Gang gesetzt, 
die auf Dienstleistungen des Kernels zugreifen müssen. Viele Systemprogramme verwenden letztlich Systemaufrufe, um ihre 
Aufgabe zu erfüllen, aber nicht alle. Ebenso wenig sollten Systemprogramme mit den einfachen Anwendungsprogrammen 
durcheinander gebracht werden, die mit vielen Betriebssystemen geliefert werden. Ein einfacher Taschenrechner, ein 
Texteditor oder ein MP3-Player ist kein Systemprogramm, sondern eine Anwendung.

#### Die Schnittstelle für Anwendungsprogramme
Jedes Betriebssystem bietet Anwendungsprogrammen die Möglichkeit, seine Dienstleistungen in Anspruch zu nehmen. Dies 
ermöglicht es Programmierern, bestimmte aufwendige und hardwareabhängige Aufgaben an das Betriebssystem zu delegieren. 
Bei den meisten aktuellen Systemen bleibt ihnen auch gar nichts anderes übrig, weil der direkte Zugriff auf die Hardware 
durch Anwendungsprogramme verhindert wird. Um eine Funktion des Betriebssystems zu verwenden, muss ein Programm einen 
Systemaufruf (System Call) durchführen. Das Betriebssystem reagiert darauf, indem es den aktuellen Prozess unterbricht, 
den geforderten Systembefehl im Kernelmodus ausführt und dessen Ergebnis an den aufrufenden Prozess zurückliefert.

Unix-Systeme bieten nur verhältnismäßig wenige, dafür aber sehr mächtige Systemaufrufe an. Einige von ihnen sind auf 
Dateien und andere Ein- und Ausgabekanäle bezogen, beispielsweise <code>create()</code> zum Erzeugen einer neuen Datei, 
<code>open()</code> zum Öffnen, <code>read()</code> zum Lesen, <code>write()</code> zum Schreiben oder 
<code>close()</code> zum Schließen. Andere Systemaufrufe beschäftigen sich mit der Prozessverwaltung; zum Beispiel 
erzeugt <code>fork()</code> einen neuen Prozess als Kopie des bestehenden, <code>kill()</code> sendet Signale an 
Prozesse, und <code>shmget()</code> fordert das Shared Memory (gemeinsame Speicherbereiche, die sich mehrere Prozesse 
zum Datenaustausch teilen) an.

Neben den eigentlichen Systemaufrufen basiert jedes Betriebssystem auf der Bibliothek der Programmiersprache, in der es 
geschrieben wurde. Nach wie vor werden die meisten Betriebssysteme zu großen Teilen in der Programmiersprache C 
geschrieben (nur einige sehr hardwarenahe Teile des Kernels werden in Assembler verfasst). Aus diesem Grund basiert die 
Arbeitsweise vieler Systembereiche auf Funktionen der C-Standardbibliothek. Unix, Windows und viele andere Systeme 
behandeln vieles aus der Sicht von Anwendungsprogrammierern recht ähnlich, weil es mithilfe der entsprechenden 
Bibliotheksroutinen realisiert wurde.

Ein Beispiel soll an dieser Stelle genügen, um einen Eindruck vom Einfluss der C-Standardbibliothek zu geben: Fast alle 
Betriebssysteme speichern Datum und Uhrzeit als die Anzahl der Sekunden seit dem 
<code>01. Januar 1970, 00:00 Uhr UTC</code>. Dieses Datum wird als EPOCH bezeichnet, weil es als der »epochemachende« 
Erfindungszeitpunkt von Unix gilt. Diese Art der Speicherung von Datum und Uhrzeit ist in der C-Bibliotheksdatei 
<code>time.h</code> definiert.

Unter Windows gibt es eine äußerst umfangreiche Betriebssystemschnittstelle, die Win32 API. Sie besteht aus Tausenden 
von Befehlen, von denen allerdings nicht alle echte Systemaufrufe sind. Viele von ihnen sind Bibliotheksfunktionen, die 
beispielsweise den Zugriff auf die Bestandteile der grafischen Benutzeroberfläche ermöglichen. Win32 steht übrigens für 
32-Bit-Windows, in Abgrenzung zu dem längst untergegangenen 16-Bit-Windows, dessen letzte Version Windows 3.11 war. Alle 
Privatkunden-Versionen seit Windows 95 und alle professionellen Versionen seit der ersten NT-Version gehören zur 
Win32-Familie; Windows XP, Windows Vista, Windows 7, 8 und 10 sowie die zugehörigen Server-Versionen sind auch in 
64-Bit-Versionen für neuere Generationen der Intel- und AMD-Prozessoren verfügbar.

#### Die Benutzeroberfläche
Es gibt zwei grundlegende Arten von Benutzeroberflächen: die Konsole oder Kommandozeile und die grafische Oberfläche. 
Beide dienen dazu, mit dem Betriebssystem zu kommunizieren, und stellen ihre Ein- und Ausgabefähigkeiten auch 
Anwendungsprogrammen zur Verfügung.

Eine Kommandozeilenoberfläche wird (in Abgrenzung zum Kernel) auch Shell genannt. Um zu ermitteln, welche Befehle, von 
der Shell unterstützt werden, hält die, Windows-Konsole einen Befehl namens <code>help</code> bereit, der eine Liste 
aller Befehle mit einer kurzen Beschreibung anzeigt. <code>help BEFEHL</code> zeigt dagegen eine ausführliche 
Beschreibung eines einzelnen Befehls an. Unter Unix heißt die entsprechende Anweisung <code>man BEFEHL</code>. Das hat 
übrigens nichts mit dem dummen Klischee zu tun, dass Unix »nur was für Männer« sei – <code>man</code> ist einfach die 
Abkürzung für Englisch: manual, also Handbuch.

Die unter Windows verwendete Konsole entspricht noch heute weitgehend der Benutzeroberfläche von MS-DOS. Die Befehle, 
die eingegeben werden können, sind fast alle kompatibel mit den alten DOS-Befehlen. Allerdings wurde inzwischen eine 
Reihe von Komfortfunktionen eingebaut, die die Arbeit mit der Windows-Kommandozeile erleichtern.

Unix-Shells sind allerdings im Vergleich zur Windows-Shell erheblich komfortabler. Das liegt natürlich zum Teil daran, 
dass die zugrunde liegenden Systembefehle, die aufgerufen werden können, mächtiger sind als die Windows-Konsolenbefehle. 
Aber auch die Shell selbst hat mehr Bequemlichkeit zu bieten als unter Windows. Beispielsweise wird unter Unix schon 
seit Langem die Eingabevervollständigung angeboten – wenn Befehle oder Dateinamen eingegeben werden, kann die 
Tabulator-Taste gedrückt werden, um einen begonnenen Namen zu ergänzen, falls er bereits eindeutig ist. Microsoft hat 
dieses Feature erst unter Windows 2000 eingeführt.

Grafische Benutzeroberflächen gibt es inzwischen für jedes Betriebssystem, und auch unter Linux und anderen 
Unix-Systemen ist es heutzutage üblich, dass gleich das GUI gestartet wird, wenn der Rechner bootet. In einer grafischen 
Oberfläche werden die einzelnen Programme und Dokumente in Fenstern dargestellt, die frei über den Bildschirm 
verschoben, vergrößert und verkleinert und in einer beliebigen Stapelreihenfolge angeordnet werden können. Mit einer 
Maus wird ein Zeiger über diese Oberfläche bewegt und es können Menübefehle ausgewählt, Schaltflächen angeklickt oder 
Symbole verschoben werden.

Unter Linux kann eine von vielen verschiedenen grafischen Oberflächen ausgesucht werden. Die grundlegenden 
Grafikfähigkeiten werden von einer Komponente namens XWindow-Server oder kurz X-Server bereitgestellt, darauf aufbauend 
läuft ein Window-Manager oder ein moderner, voll ausgestatteter Desktop. Die beiden häufigsten Desktops sind KDE und 
GNOME.

Windows und macOS lassen einem dagegen keine Wahl bei der Entscheidung für ein bestimmtes GUI, weil es ein fester 
Bestandteil des Betriebssystems selbst ist. Selbst einige der elementarsten Programme sind so geschrieben, dass sie 
diese eine Oberfläche voraussetzen. Beide Hersteller haben ihre grafischen Oberflächen in der neuesten Version ihrer 
Betriebssysteme modernisiert; macOS verwendet eine elegante Oberfläche namens Aqua, die Windows-10-Oberfläche (seit 
Windows 8 verfügbar) wird Metro genannt.

Für macOS ist auch ein X-Server verfügbar, sodass der reichhaltige Bestand X-basierter Software, der für andere 
Unix-Versionen vorhanden ist, bei Bedarf auch unter macOS zur Verfügung steht. Bis Mac OS X 10.5 wurde die Software 
offiziell von Apple selbst angeboten und danach als Community Edition weitergeführt. Unter 
<a href="http://xquartz.macosforge.org/landing/">http://xquartz.macosforge.org/landing/</a> kann die Software 
heruntergeladen werden. Auch für Windows gibt es übrigens verschiedene X-Server von Drittanbietern.

### Prozessverwaltung
Jedes moderne Betriebssystem ist in der Lage, scheinbar mehrere Aufgaben gleichzeitig auszuführen. Diese Fähigkeit wird 
allgemein als Multitasking bezeichnet. Es geht dabei nicht nur um den bequemen Nebeneffekt, dass mehrere 
Anwendungsprogramme geöffnet sein können und zwischen ihnen hin- und hergeschaltet werden kann, sondern vor allem um 
Aufgaben, die das Betriebssystem im Hintergrund erledigen muss, während nur eines dieser Programme verwendet wird.

Jede der einzelnen gleichzeitig stattfindenden Aufgaben wird unter den meisten Betriebssystemen durch einen Prozess 
realisiert. Einem Prozess stehen aus seiner eigenen Sicht alle Ressourcen des Rechners exklusiv zur Verfügung: die 
gesamte ungeteilte Rechenzeit des Prozessors, der vollständige Arbeitsspeicher und der alleinige Zugriff auf sämtliche 
Ein- und Ausgabekanäle. Es ist Sache des Betriebssystems, die Ressourcen hinter den Kulissen zu verteilen. Ein Prozess, 
der auf eine Ressource wartet, muss in einen Wartezustand versetzt und später wieder aufgerufen werden.

Dieser Service eines Betriebssystems erleichtert es Anwendungsprogrammierern, sich auf ihre eigentlichen Aufgaben zu 
konzentrieren. Wenn eine Bedingung eintritt, für die ein bestimmter Prozess nicht zuständig ist, übernimmt das System 
automatisch die Kontrolle, legt den Prozess schlafen, löst das anstehende Problem und ruft den Prozess anschließend 
wieder auf.

#### Das Unix-Prozessmodell
Besonders gut verständlich ist das Prozessverwaltungssystem von Unix. Für Unix-Prozesse gelten die folgenden Aussagen:
<list>
    <li>
        Jeder Prozess ist durch eine eindeutige ganzzahlige Nummer gekennzeichnet, seine Prozess-ID (PID).
    </li>
    <li>
        Der erste Prozess, der auf dem Rechner gestartet wird, heißt <code>init</code>, hat die PID 1 und erzeugt alle 
        anderen Prozesse direkt oder indirekt.
    </li>
    <li>
        Jeder Prozess läuft entweder im Kernelmodus oder im Benutzermodus, und zwar ein für alle Mal. Keiner kann den 
        Modus nachträglich wechseln. Ein Anwendungsprogramm kann niemals selbst einen Prozess starten, der im 
        Kernelmodus läuft – dafür gibt es Systemaufrufe.
    </li>
    <li>
        Ein neuer Prozess wird durch einen speziellen Systemaufruf namens <code>fork()</code> erzeugt. Dieser 
        Systemaufruf erzeugt eine identische Kopie des Prozesses, der ihn gestartet hat – der neue Prozess kann sich 
        sogar daran »erinnern«, <code>fork()</code> aufgerufen zu haben. Lediglich die PID ist eine andere. In der Regel 
        wird der neue Prozess anschließend für eine neue Aufgabe eingesetzt.
    </li>
    <li>
        Jeder Prozess besitzt einen Parent-Prozess. Dabei handelt es sich um denjenigen Prozess, der ihn aufgerufen hat. 
        Wenn der Parent-Prozess vor dem Child-Prozess beendet wird, wird das Child dem Ur-Prozess <code>init</code> 
        zugewiesen. Auf diese Weise wird sichergestellt, dass Prozesse auch weiterhin einen Parent-Prozess besitzen.
    </li>
    <li>
        Wird ein Child-Prozess dagegen beendet, wird er nicht komplett aus dem Speicher und aus der Prozesstabelle 
        entfernt, sondern bleibt mit dem speziellen Status <code>defunct</code> (außer Betrieb) als sogenannter 
        Zombie-Prozess bestehen. In diesem Zustand bleiben die Zombies, bis der Parent-Prozess den Systemaufruf 
        <code>waitpid()</code> durchführt; dies wird als Reaping (Ernte) bezeichnet. Auf diese Weise kann der Parent den 
        Exit-Status seiner Child-Prozesse untersuchen.
    </li>
    <li>
        Jeder Prozess reagiert auf eine Reihe verschiedener Signale. Diese Signale sind durchnummeriert, in der Praxis 
        werden jedoch symbolische Namen für diese Signale verwendet, die irgendwo in der Betriebssystembibliothek 
        definiert sind. Signale werden mithilfe des Systemaufrufs <code>kill()</code> an einen Prozess gesandt. Der 
        etwas seltsame Name rührt daher, dass das Standardsignal den Prozess auffordert, sich zu beenden, falls kein 
        anderes Signal angegeben wird. Wichtige Signale sind etwa folgende: <code>SIGTERM</code> beendet den Prozess 
        normal, <code>SIGKILL</code> erzwingt einen sofortigen Abbruch, <code>SIGHUP</code> (Hangup) weist darauf hin, 
        dass eine Verbindung unterbrochen wurde (etwa eine Netzwerkverbindung), und <code>SIGALRM</code> zeigt an, dass 
        ein Timer-Alarm ausgelöst wurde, den Programmierer wiederum verwenden können, um einen Prozess nach einer 
        definierten Zeit wieder zu wecken.
    </li>
    <li>
        Ein Prozess kann jederzeit selbst die Kontrolle abgeben, indem er den Systemaufruf <code>pause()</code> 
        durchführt. In diesem Fall kann er durch ein Signal wieder geweckt werden.
    </li>
    <li>
        Prozesse im Benutzermodus können auch von außen unterbrochen und später wieder aufgenommen werden.
    </li>
</list>

Wenn ein Prozess unterbrochen wird, muss der Systemzustand, der derzeit herrscht, gespeichert werden, um ihn bei 
Wiederaufnahme erneut herzustellen. Dazu gehören vor allem die Inhalte der Prozessorregister und der Flags sowie eine 
Liste aller geöffneten Dateien. Wenn ein Prozess weiterläuft, findet er die Systemumgebung also genau so vor, wie er sie 
verlassen hat.

Neben der Prozess-ID besitzt jeder Prozess in einem Unix-System eine User-ID (UID) und eine Group-ID (GID). Diese beiden 
Informationen sind für die Systemsicherheit wichtig: Die User-ID kennzeichnet den Benutzer, dem der Prozess gehört, die 
Group-ID die Benutzergruppe. Ein Benutzer ist entweder eine bestimmte Person oder eine vom Betriebssystem definierte 
Einheit; einer Gruppe können beliebig viele Benutzer angehören. Ein Prozess reagiert nur auf Signale, die von einem 
anderen Prozess mit derselben UID und GID aus versandt wurden. Die einzige Ausnahme sind die UID und GID 0, die dem 
Superuser root vorbehalten sind. Dieser spezielle Benutzer darf auf einem Unix-System alles, also auch jeden Prozess 
beenden, unterbrechen oder anderweitig steuern.

Mithilfe des Befehls ps kann auf einer Unix-Konsole angezeigt werden, welche Prozesse gerade laufen. Angezeigt werden 
die PID, die UID, die GID und der Pfad des Prozesses. Der Pfad ist die genaue Ortsangabe der Programmdatei, die in dem 
entsprechenden Prozess ausgeführt wird.

Windows verwendet ein etwas komplexeres Prozessmodell. Vor allem wird ein neuer Prozess durch einen Systemaufruf namens 
CreateProcess()erzeugt, der keine exakte Kopie des aufrufenden Prozesses erzeugt, sondern einen »leeren« Prozess, dem 
anschließend eine Aufgabe zugewiesen werden muss. Außerdem ist jeder Prozess im Benutzermodus mit einer numerischen 
Priorität ausgestattet. Diese entscheidet im Zweifelsfall, welcher Prozess Vorrang hat. Die Liste der laufenden Prozesse 
wird auf der Registerkarte Prozesse des Task-Managers angezeigt. Hier besteht auch die Möglichkeit, abgestürzte Prozesse 
zwangsweise zu beenden.

Prozesse haben den Vorteil, dass sie vollkommen voneinander abgeschirmt laufen können: Sie besitzen getrennte 
Speicherbereiche und können einander nicht in die Quere kommen. Manchmal kann dieser Vorteil jedoch auch ein Nachteil 
sein, denn mitunter müssen Prozesse miteinander kommunizieren. Eine einfache, aber auf wenige »Wörter« beschränkte 
Möglichkeit ist die bereits erwähnte Verwendung von Signalen.

Eine andere Option besteht in der Verwendung sogenannter Pipes, die die Ausgabe eines Programms und damit eines 
Prozesses mit der Eingabe eines anderen verknüpfen. Pipes werden in den Konsolen von Unix und Windows häufig eingesetzt, 
um die Ausgabe eines Programms durch ein anderes zu filtern, können aber auch aus Programmen heraus geöffnet werden.

Die effizienteste Möglichkeit der Kommunikation zwischen Prozessen heißt Inter Process Communication oder System V IPC. 
Obwohl sie mit System V eingeführt wurde und nicht zum POSIX-Standard gehört, ist sie inzwischen in fast allen 
Unix-Varianten verfügbar, zum Beispiel auch unter Linux. Im Wesentlichen verwendet die IPC zwei verschiedene 
Mechanismen: In sogenannte Nachrichtenwarteschlangen (Message Queues) kann ein Prozess schreiben; ein anderer kann 
sequenziell daraus lesen. Gemeinsame Speicherbereiche (Shared Memory) sind dagegen einfacher zu handhaben: Was ein 
Prozess in diesem Speicherbereich ablegt, können andere beliebig oft lesen oder ändern.

Eine eingeschränkte Form der Verständigung zwischen Prozessen findet schließlich durch Semaphore statt. Dabei handelt es 
sich im Grunde um einen Zähler in einem gemeinsamen Speicherbereich, der von verschiedenen Prozessen reserviert 
beziehungsweise freigegeben werden kann. Beim Reservieren wird der Zähler um 1 heruntergezählt, sofern er noch größer 
als 0 ist, beim Freigeben wird 1 bis zu einem festgelegten Maximalwert addiert. So können mehrere Prozesse 
beispielsweise eine beschränkte Anzahl von Ressourcen gemeinsam nutzen.


#### Deadlocks

#### Threads

### Speicherverwaltung

### Dateisysteme

#### Das virtuelle Unix-Dateisystem

#### Das virtuelle Windows-Dateisystem