# Zug (city): law history in git

The municipal law of the city of Zug (Stadt Zug, canton of Zug, Switzerland) as a git history: one file per article, one commit per amending act on the day it took effect, and the amending act as the commit's author. `git blame` names the act behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law). The law of the canton of Zug is in [lexifina/switzerland-zug-law](https://github.com/lexifina/switzerland-zug-law); federal law is in [lexifina/switzerland-law](https://github.com/lexifina/switzerland-law).

The text is in German, exactly as the city publishes it.

## What this repository holds

80 acts with 129 versions so far: the Gemeindeordnung (the city's charter) first, then the city's other enactments in force (ordinances, regulations, tariffs and decisions), in the order of the systematic collection, added in parts of about 50. Agreements, concessions, directives and repealed acts are not included.

| Folder | Act | Versions | History |
| --- | --- | ---: | --- |
| `1-1-1/` | Gemeindeordnung (SRS 1.1-1) | 2 | as enacted, then each consolidated version: 1 July 2005 to 14 May 2024 |
| `1-2-1/` | Verordnung über die Aktenführung und das Stadtarchiv (SRS 1.2-1) | 1 | as enacted, 1 January 2016 |
| `1-4-1-1/` | Einwohnerdienste: Wahl- und Abstimmungslokale; Anpassung Urnenöffnungszeiten (SRS 1.4-1.1) | 1 | as enacted, 1 January 2025 |
| `1-4-2/` | Verordnung über die politische Aussenwerbung (SRS 1.4-2) | 1 | as enacted, 30 January 2018 |
| `1-5-1-geschaftsordnung-gso/` | Geschäftsordnung des Grossen Gemeinderates der Stadt Zug (SRS 1.5-1) | 1 | one version (the oldest available), 1 January 2021 |
| `1-5-3/` | Reglement über die Entschädigungen der Behörden und Kommissionsmitglieder der Stadt Zug (SRS 1.5-3) | 1 | one version (the oldest available), 1 January 2021 |
| `1-6-1-1-go-stadtrat/` | Geschäftsordnung des Stadtrates von Zug (SRS 1.6.1-1) | 6 | oldest version available, then each consolidated version: 1 July 2021 to 1 May 2025 |
| `1-6-1-2-stadtratsreglement/` | Reglement über das Dienstverhältnis, die Besoldung und die berufliche Vorsorge des Stadtrates von Zug (SRS 1.6.1-2) | 2 | oldest version available, then each consolidated version: 27 September 2009 to 1 January 2026 |
| `1-6-1-3/` | Informatik: Verrechnungsansätze der Dienstleistungen für öffentliche Verwaltungen (SRS 1.6.1-3) | 1 | as enacted, 22 March 2005 |
| `1-6-2-1-delegationsverordnung/` | Verordnung über die Delegation von Entscheidkompetenzen an die Departemente (SRS 1.6.2-1) | 4 | oldest version available, then each consolidated version: 1 January 2017 to 1 January 2025 |
| `1-6-2-1-11/` | Organisation: Departementsentscheid Kompetenzdelegation Sozialhilfe; Kompetenzdelegation an die Abteilung Soziales und Gesellschaft (SRS 1.6.2-1.11) | 2 | as enacted, then each consolidated version: 1 January 2024 to 1 May 2025 |
| `1-6-3-1-vo-kuko/` | Verordnung über die Kulturkommission (SRS 1.6.3-1) | 2 | as enacted, then each consolidated version: 1 March 2000 to 1 July 2024 |
| `1-6-3-2/` | Verordnung über die Nachhaltigkeitskommission (SRS 1.6.3-2) | 2 | as enacted, then each consolidated version: 1 June 2013 to 1 October 2022 |
| `1-6-3-3/` | Verordnung über die Stadtbildkommission (SRS 1.6.3-3) | 2 | as enacted, then each consolidated version: 1 January 2021 to 1 January 2025 |
| `1-6-3-5/` | Verordnung für die Personalkommission der Einwohnergemeinde Zug (SRS 1.6.3-5) | 1 | as enacted, 5 July 1988 |
| `1-6-3-6/` | Verordnung über die Grundstückgewinnsteuerkommission (SRS 1.6.3-6) | 1 | one version (the oldest available), 1 January 2018 |
| `1-6-3-7-energieverordnung/` | Verordnung über die Organisation der Energiekommission (SRS 1.6.3-7) | 2 | as enacted, then each consolidated version: 1 May 2000 to 1 January 2026 |
| `1-7-1-1-pr/` | Personalreglement (SRS 1.7.1-1) | 2 | as enacted, then each consolidated version: 1 January 2010 to 1 January 2024 |
| `1-7-1-1-1-pv/` | Personalverordnung (SRS 1.7.1-1.1) | 3 | oldest version available, then each consolidated version: 1 January 2018 to 1 August 2025 |
| `1-7-1-2-glaz-verordnung/` | Verordnung über die gleitende Arbeitszeit (GLAZ) in der Stadtverwaltung Zug (SRS 1.7.1-2) | 1 | one version (the oldest available), 1 January 2010 |
| `1-7-1-3/` | Erlass von Grundsätzen zum Schutz der persönlichen Integrität am Arbeitsplatz (SRS 1.7.1-3) | 1 | as enacted, 2 December 1997 |
| `1-7-2-1-entschadigungsverordnung/` | Verordnung über besondere Entschädigungen an das Personal der Stadt Zug (SRS 1.7.2-1) | 2 | as enacted, then each consolidated version: 1 January 2021 to 1 January 2025 |
| `1-7-2-1-1-9/` | Personal: Gehälter 2025; Regelung der Teuerungszulage an das städtische Personal (SRS 1.7.2-1.1.9) | 3 | as enacted, then each consolidated version: 1 January 2023 to 5 November 2024 |
| `1-7-2-2-spesenverordnung/` | Verordnung über die Spesenentschädigungen an das Personal der Stadt Zug (SRS 1.7.2-2) | 1 | as enacted, 1 August 2025 |
| `4-1-3-reglement-betreuung/` | Reglement über die familienergänzende Betreuung von Kindern (SRS 4.1-3) | 1 | one version (the oldest available), 1 January 2019 |
| `4-1-3-1-vo-gutscheine/` | Verordnung über Gutscheine für die Betreuung in Kindertagesstätten (SRS 4.1-3.1) | 4 | as enacted, then each consolidated version: 1 January 2019 to 1 August 2026 |
| `4-1-4-spielgruppenrichtlinien/` | Richtlinien für die Anerkennung von Spielgruppen und die Ausrichtung von städtischen Beiträgen (SRS 4.1-4) | 2 | as enacted, then each consolidated version: 1 January 2017 to 1 January 2025 |
| `4-2-1-1/` | Schul- und Disziplinarordnung der Stadtschulen Zug (SRS 4.2.1-1) | 1 | as enacted, 14 March 2009 |
| `4-2-1-7-tagesschulreglement/` | Reglement über die Tagesschule der Stadt Zug (SRS 4.2.1-7) | 1 | as enacted, 1 August 2014 |
| `4-2-1-7-1-tagesschulverordnung/` | Verordnung über die Tagesschule der Stadt Zug (SRS 4.2.1-7.1) | 1 | as enacted, 1 August 2014 |
| `4-2-2-1/` | Reglement über die Musikschule der Stadt Zug (SRS 4.2.2-1) | 1 | as enacted, 1 February 1992 |
| `4-2-2-1-1-musikschulvo/` | Verordnung über die Musikschule der Stadt Zug (SRS 4.2.2-1.1) | 1 | as enacted, 1 August 2018 |
| `4-2-3-1/` | Reglement über den Schulzahnarztdienst (SRS 4.2.3-1) | 1 | one version (the oldest available), 1 August 2021 |
| `4-2-3-1-1/` | Verordnung über den Schulzahnarztdienst (SRS 4.2.3-1.1) | 2 | as enacted, then each consolidated version: 1 August 2003 to 1 August 2021 |
| `4-7-1-kulturforderungsreglement-kfr/` | Reglement über die Kulturförderung (SRS 4.7-1) | 2 | as enacted, then each consolidated version: 20 February 2001 to 1 January 2024 |
| `4-7-3/` | Bibliotheks-Vertrag (SRS 4.7-3) | 1 | as enacted, 1 March 2017 |
| `4-7-3-1/` | Verwaltungs-Reglement über die Verwaltung der Stadt- und Kantonsbibliothek Zug (SRS 4.7-3.1) | 1 | as enacted, 21 January 1986 |
| `4-7-3-2/` | Benützungsordnung der Stadt- und Kantonsbibliothek Zug (SRS 4.7-3.2) | 1 | one version (the oldest available), 16 August 2005 |
| `5-3-1/` | Feuerwehrreglement der Stadt Zug (SRS 5.3-1) | 2 | as enacted, then each consolidated version: 1 January 2014 to 1 January 2024 |
| `5-3-1-1/` | Feuerwehr: Verrechnung von Einsätzen und Dienstleistungen der Feuerwehr ab 1. März 2024; Verrechnungsansätze (SRS 5.3-1.1) | 3 | as enacted, then each consolidated version: 1 January 2015 to 1 March 2024 |
| `5-5-1/` | Gemeindeführungsstab: Organisation; Anpassung Organigramm und Pflichtenheft (SRS 5.5-1) | 1 | as enacted, 1 January 2025 |
| `6-1-1/` | Finanzverordnung (SRS 6.1-1) | 1 | as enacted, 1 January 2018 |
| `6-4-3-sponsoringrichtlinien/` | Richtlinien über die Mitfinanzierung von Aufgaben der Stadt Zug durch Sponsoring (SRS 6.4-3) | 1 | as enacted, 26 May 2015 |
| `6-4-7/` | Gebührenordnung für die Bereiche Nutzung des öffentlichen Raumes, Taxistandplätze, Gastgewerbe und Strafbefehlsverfahren (SRS 6.4-7) | 1 | one version (the oldest available), 1 January 2019 |
| `6-6-1-anlagenbenutzungsverordnung/` | Verordnung über die Benützung der Sportanlagen, Schulanlagen, Mehrzwecksäle sowie Militär- und Zivilschutzräume (SRS 6.6-1) | 1 | one version (the oldest available), 1 August 2020 |
| `6-6-3/` | Verordnung über die Vermietung von Musikräumen der Stadt Zug (SRS 6.6-3) | 1 | as enacted, 4 November 1997 |
| `6-6-4-badeordnung-hallenbader/` | Badeordnung für die öffentlichen Hallenbäder der Stadt Zug (SRS 6.6-4) | 1 | one version (the oldest available), 1 August 2017 |
| `6-6-6/` | Verordnung über die Benützung der Schiessanlagen im Choller (SRS 6.6-6) | 2 | oldest version available, then each consolidated version: 1 December 2013 to 1 January 2023 |
| `6-6-7/` | Benützungsordnung für die Seebäder (SRS 6.6-7) | 2 | oldest version available, then each consolidated version: 1 May 2021 to 1 May 2024 |
| `7-1-1/` | Bauordnung der Stadt Zug (SRS 7.1-1) | 3 | oldest version available, then each consolidated version: 22 March 2021 to 3 November 2023 |
| `7-1-1-1/` | Gebührenordnung für das Planungs- und Baubewilligungsverfahren (SRS 7.1-1.1) | 1 | as enacted, 1 January 2018 |
| `7-1-1-2/` | Verordnung über die Zone für preisgünstigen Wohnungsbau (SRS 7.1-1.2) | 4 | oldest version available, then each consolidated version: 24 March 2020 to 1 November 2025 |
| `7-1-1-3-altstadtr/` | Altstadtreglement (SRS 7.1-1.3) | 1 | as enacted, 1 April 2016 |
| `7-1-1-4/` | Reglement über die Planung und Erstellung von Hochhäusern (SRS 7.1-1.4) | 1 | as enacted, 7 May 2018 |
| `7-1-1-5/` | Parkplatzreglement (SRS 7.1-1.5) | 1 | as enacted, 22 July 2010 |
| `7-3-1-larmschutzreglement-lsr/` | Reglement über den Schutz vor Lärmimmissionen (SRS 7.3-1) | 2 | as enacted, then each consolidated version: 16 June 1972 to 1 September 2023 |
| `7-3-2/` | Verordnung über die Feuerungskontrolle (SRS 7.3-2) | 2 | oldest version available, then each consolidated version: 1 October 2010 to 1 February 2022 |
| `7-4-3-energier/` | Energiereglement (SRS 7.4-3) | 2 | as enacted, then each consolidated version: 1 January 2011 to 1 January 2022 |
| `7-4-3-1/` | Energiekommission: Energie-Förderprogramm 2025 (SRS 7.4-3.1) | 3 | as enacted, then each consolidated version: 1 January 2023 to 1 January 2025 |
| `7-4-4/` | Abwasserreglement (SRS 7.4-4) | 1 | as enacted, 1 January 2008 |
| `7-6-1/` | Reglement über Strassen und Wege (SRS 7.6-1) | 1 | as enacted, 6 April 2000 |
| `7-6-2/` | Reglement über die Bestellung von Leistungen des öffentlichen Verkehrs (SRS 7.6-2) | 1 | as enacted, 1 January 2021 |
| `7-6-2-1/` | Öffentlicher Verkehr: Angebotsbeschluss gemäss § 2 des Reglements über die Bestellung von Leistungen des öffentlichen Verkehrs (SRS 7.6-2.1) | 1 | as enacted, 28 February 2023 |
| `7-6-3/` | Reglement über die Aussenwerbung (SRS 7.6-3) | 1 | as enacted, 1 February 2012 |
| `7-7-1-1/` | Reglement über die Benützung der öffentlichen Anlagen (SRS 7.7.1-1) | 2 | oldest version available, then each consolidated version: 1 March 2021 to 1 January 2025 |
| `7-7-1-1-1/` | Gebührenordnung für die Benützung der öffentlichen Anlagen (SRS 7.7.1-1.1) | 1 | as enacted, 1 January 2019 |
| `7-7-1-2-1/` | Richtlinien für das Sponsoring von Veranstaltungen auf öffentlichem Grund (SRS 7.7.1-2.1) | 1 | as enacted, 26 September 2000 |
| `7-7-1-2-2/` | Verordnung über die Strassenkunst (SRS 7.7.1-2.2) | 1 | one version (the oldest available), 1 January 2019 |
| `7-7-1-3/` | Verordnung über die Konzessionsgebühren für die Sondernutzung von öffentlichem Grund (SRS 7.7.1-3) | 1 | as enacted, 26 June 2007 |
| `7-7-5-1/` | Reglement über das nächtliche Dauerparkieren auf öffentlichem Grund (SRS 7.7.5-1) | 2 | as enacted, then each consolidated version: 2 July 1968 to 1 January 2025 |
| `7-7-5-2/` | Verordnung über die Parkraumbewirtschaftung (SRS 7.7.5-2) | 3 | as enacted, then each consolidated version: 1 January 2021 to 1 May 2025 |
| `7-7-5-3/` | Verordnung über die Erteilung von Zufahrtsbewilligungen (SRS 7.7.5-3) | 1 | as enacted, 1 January 2022 |
| `7-7-5-4-1/` | Organisation: Departementsentscheid Kompetenzdelegation Parkraumbewirtschaftung; Subdelegation an die Abteilung Sicherheit und Verkehr (SRS 7.7.5-4.1) | 1 | as enacted, 1 May 2025 |
| `7-7-7-1-hafenordnung/` | Betriebsreglement für den Bootshafen Zug (SRS 7.7.7-1) | 1 | as enacted, 16 November 1999 |
| `8-1-1/` | Reglement über die Langzeitpflege (SRS 8.1-1) | 1 | as enacted, 1 July 2000 |
| `8-2-1/` | Benützungsordnung Friedhof St. Michael (SRS 8.2-1) | 2 | oldest version available, then each consolidated version: 1 July 2020 to 1 January 2024 |
| `8-2-1-1/` | Gebührenordnung Friedhof St. Michael (SRS 8.2-1.1) | 2 | as enacted, then each consolidated version: 1 July 2020 to 1 January 2024 |
| `9-4-1/` | Verordnung betreffend die Einführung einer Beherbergungsabgabe (SRS 9.4-1) | 2 | oldest version available, then each consolidated version: 1 January 2007 to 1 January 2023 |
| `9-5-4/` | Taxireglement der Stadt Zug (SRS 9.5-4) | 1 | as enacted, 1 January 2017 |
| `9-5-4-2/` | Taxireglement der Stadt Zug; Richtlinien für Bussenbemessung der kommunalen Übertretungstatbestände (SRS 9.5-4.2) | 1 | as enacted, 1 January 2017 |

## Source

The SRS (systematic collection) of the city, published by the city at <https://zug.tlex.ch/>. For each act it gives every consolidated version it holds, with the day each version took effect, and a change table listing each amendment: its decision date, the day it took effect, the provision it touched and its entry in the chronological collection (CRS). Annexes the collection publishes only as separate PDF files are not included.

## Dates

- Each commit is dated at **noon, Europe/Zurich, on the day the version took effect**, as the collection gives it ("in Kraft seit / von"). The decision date of each amending act is the `Enacted:` trailer.
- An act's first commit is its oldest version in the collection. It is credited to the act as enacted only when the change table shows no amendment in force before it; otherwise it is the "oldest version available", naming the earlier amendments.
- Versions that take effect after the retrieval day are on the `zukunft` branch, never merged into `main`.
- `--before="YYYY-MM-DD"` alone uses your clock's time of day; use `T23:59:59Z` or `tools/on.py`.

## Files

`<act>/art-005.md` is Art. 5 (or § 5), `art-005a.md` Art. 5a; `ingress.md` holds the title, date and preamble; `gliederung.md` the section headings; `schluss.md` the closing formula and signatures. One paragraph or list item per line. Amendment markers (`*`), footnote numbers and the "Stand" date are left out.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the city's own text of that version, and every article's text appears in it in order.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the amending act, named by its entry in the chronological collection (CRS), with an e-mail address that cannot exist (`<act key>@zug.tlex.ch.invalid`). Where one version holds changes by several amending acts and the change table does not say which provision each one touched, the commit names them all. The committer is always Lexifina.

## Limits

This is not an official publication. The binding text is the one the city publishes as binding. The history starts with the oldest consolidated version the collection holds for each act, which for many acts is later than the act's enactment. Only the acts listed above are included.
