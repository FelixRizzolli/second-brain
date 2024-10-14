# Worum handelt es sich hier?

SecondBrain ist ein Konzept das den Wunsch entstammt, einen Teil der eigenen Gedächtnisleistung auslagern zu können. Das
betrifft: Dinge, an die man sich später erinnern will; Aufgaben, die noch zu erledigen sind; Interessante oder nützliche
Informationen, denen man begegnet und die man “für später” abspeichern möchte; Ergebnisse aus Recherchearbeit. Dieses
Konzept setze ich wie folgt um:

- Mit Writerside erstelle ich eine Dokumentation welche ich durch eine GitHub Action auf GitHub Pages deploye. Dort
  kommt all jenes wissen, welches ich als interessant oder nützlich empfinde. Dabei schreibe ich hauptsächlich
  Zusammenfassungen von Büchern, Videos und Artikel.
- GitHub Projects verwende ich um interessante Artikel, Bücher, Videos usw. "für später" abzuspeichern. Dabei erstelle
  ich pro Buch/Artikel/... ein Issue, welches ich vor habe zusammengefasst in meine Dokumentation einzubauen.

# Struktur

## Projekte

Für jedes Hauptthema gibt es ein eigenes GitHub Projekt. Diesem Projekt werden die dazugehörigen Issues zugewiesen und
man kann deren Status verfolgen.

| Thema          | Beschreibung                                                                                                                                                                          | Link                                               |
|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------|
| Verbesserungen | In diesem Projekt werden Anpassungen des Standards der Dokumentation, Ideen zur verwendung der von Writerside bereitgestellten Tools, sowie Verbesserungen des Inhaltes festgehalten. | https://github.com/users/FelixRizzolli/projects/3  |
| Informatik     | Mainframeentwicklung, Anwendungsentwicklung, Webentwicklung, Softwareentwicklung im Allgemeinen, Datenbanken, Betriebssysteme, Design, Netzwerktechnik, Arbeiten mit Anwendungen, ... | https://github.com/users/FelixRizzolli/projects/4  |
| Philosophie    | Prosuktivitätssteigerung, Kommunikation, Philosophische Ansätze wie Stoizismus                                                                                                        | https://github.com/users/FelixRizzolli/projects/6  |
| Wirtschaft     | Die Börse, Anlageprodukte, ...                                                                                                                                                        | https://github.com/users/FelixRizzolli/projects/7  |
| Gesundheit     | Ernährung, Sport, Unverträglichkeiten                                                                                                                                                 | https://github.com/users/FelixRizzolli/projects/10 |
| Truthiness     | Was ist Wahr, was ist Falsch?; Wie überprüfe ich Informationen?; Mythen und Bullshit wie Granderwasser & Homöopathie                                                                  | https://github.com/users/FelixRizzolli/projects/11 |
| Sprachen       | Wie lerne ich Sprachen?, Deutsch, Italienisch, Englisch                                                                                                                               | https://github.com/users/FelixRizzolli/projects/8  |
| Mathematik     | Analysis, Statistik, Diskrete Mathematik, ...                                                                                                                                         | https://github.com/users/FelixRizzolli/projects/5  |

## Items & Issues

Ein GitHub Projekt Item ist meistens nur eine Informationsquelle, die mein interesse geweckt hat, und welche ich als
relevant genug empfinde, sie zusammengefasst ins SecondBrain zu übertragen. Vor deren Zusammenfassung analysiere ich das
Item, breche es auf mehrere Unteraufgaben herunter und füge diese mit weiteren Details in ein daraus entstehenden
GitHub Issue ein.

### Item Titel Standard

Struktur:

`(QUELLENTYP) Quellendetais Kommasepariert`

Beispiele:

`(BUCH) 978-1544512266, "Can't hurt me", David Goggins`

`(WEBSITE) https://en.wikipedia.org/wiki/Poverty, "Poverty"`

`(VIDEO) https://www.youtube.com/watch?v=r6tH55syq0o, "How programmers flex on each other", Fireship`

`(PODCAST) https://www.ardaudiothek.de/episode/quarks-science-cops/die-akte-wuenschelrute-gefaehrliche-wasseradern-und-erdstrahlen/wdr/12551419/, "Die Akte Wünschelrute: Gefährliche Wasseradern und Erdstrahlen?"`

### Issue

#### Titel

| Quellentyp | Titelzusammensetzung                     |
|------------|------------------------------------------|
| Buch       | "Buchtitel", Buchautoren mit & Separiert |
| Video      | "Videotitel", Kanal                      |
| Podcast    | "Podcasttitel", Kanal                    |
| Webseite   | "Webseitentitel" (Webseitendomäne)       |

#### Beschreibung

Die Beschreibung wird aufgeteilt auf "Details" und "Inhaltsverzeichnis / Aufgaben". Beim Inhaltsverzeichnis wird das
Issue auf mehreren kleineren Aufgaben heruntergebrochen. Die Details bestehen abhängig vom Quellentyp aus
unterschiedlichen informationen; nur der Inhaltstyp ist bei allen gegeben.

- **BUCH**
    - ISBN
    - Titel
    - Autor
    - Erscheinungsjahr (JJJJ)
    - Seiten
- **VIDEO**
    - Link
    - Titel
    - Kanal
    - Erscheinungsdatum (JJJJ-MM-TT)
    - Dauer
- **PODCAST**
    - Link
    - Titel
    - Kanal
    - Erscheinungsdatum (JJJJ-MM-TT)
    - Dauer
- **WEBSEITE**
    - Link
    - Titel
    - Domäne
    - Erscheinungsdatum (JJJJ-MM-TT)

## Seitenaufbau

### Inhaltsseite

### Titelseite
