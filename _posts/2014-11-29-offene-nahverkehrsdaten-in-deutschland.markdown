---
layout: post_14
title:  "Nahverkehrsdaten in Deutschland – Status Quo"
author: Stefan Kaufmann
category: 14
---

 * Nicht das Auto, sondern der ÖPNV ist die Zukunft. Aber der ist nur etwas für Kenner! Das darf nicht sein.
 * Soll-Fahrplandaten sind i.d.R. in Deutschland immer noch „streng geheim“
   * Außerdem Fortmatvielfalt: HAFAS, DIVA, IVU.pool, DINO, Geofox, …
 * Der VDV hat eine Empfehlung zu Open Data in der VDV-Schrift 7030
   * PDF kostet 30 Euro
   * Quintessenz: Sollfahrpläne als Open Data soll man lieber nicht anbieten, sondern bloß Schnittstellen (wird vom VDV „Open Service“ genannt)
 * Die offiziellen Schnittstellen können aber immer noch vieles nicht
   * Beispiel: Ulmer Buslinie 15 („Geheimtipp“) fährt von Uni Nord nach Weststadt. Auskunft berücksichtigt aber in der Regel nur die Abfahrt von der Uni Süd. Die 15 taucht so nicht auf.
     * Ortsunkundige finden nicht den Weg durch den Campus (Uni Süd → Uni Nord), d.h. für „Normal-Fahrgäste“ ist die Beauskunftung ohne Berücksichtigung der Uni Nord u.U. ganz gut so. Expert_innen, die sich in der Uni zurechtfinden, ärgert das aber.
   * Beispiel: Ich habe ein Semesterticket (oder einen anderen Zeitfahrschein)
     * Welches Ticket brauche ich von A nach C, wenn mein Zeitfahrschein von A bis B gilt, und von B bis C ein anderer Verbundtarif gilt? Z.B. von Ulm nach Stuttgart: Bis Geislingen gilt das DING-Semesterticket, ab Geislingen bis Stuttgart der VVS-Tarif
     * DB sagt bei einer Abfrage Geislingen→Stuttgart: VVS verkaufe ich nicht, Preisauskunft nicht möglich!

# Was sind eigentlich ÖPNV-Daten?

Im ÖPNV fällt eine ganze Menge an Daten an:

   * Haltepunkte
   * Wegestrecken
   * Zeitstrecken
   * Betriebspunkte
   * Linien
   * Wegemuster (Journey Patterns)
   * Fahrten
   * Tarife
   * Umläufe
   * Dienstplanung

Viele dieser Daten sind ganz furchtbar geheim, denn ein Konkurrent könnte bei einer Neuauschreibung aus der jahrelangen Erfahrung des derzeitigen Anbieters bei der Umlaufplanung profitieren und einfach dessen erprobte Umläufe übernehmen. Oder noch „schlimmer“: Auslastungsstatistiken verwenden, um sich bei einer Ausschreibung auf die Filetstücke zu bewerben. (Was die Wettbewerber davon abhalten soll, einfach selber im Bus mitzufahren und zu zählen, hat mir noch niemand erklären können).

Realitätscheck: Die Lieblings-ÖPNV-Datenaustauschformate (nach Häufigkeit absteigend sortiert) sind:

   * liniertes Papier/Excel
   * HAFAS
   * DIVA (DING verwendet DIVA; aber DIVA-Modellierung eines bayerischen Bus-Fahrplanzulieferers ist inkompatibel zur DIVA-Modellierung des DING!)
   * ÖPNV-Datenmodell des VDV

 * DIVA
   * unlesbares Monster
   * siehe Diplomarbeit von Stefan Kaufmann
   * Gauss-Krüger-Abbildung mit speziellem Koordinatenursprung
   * Nordwert mit eigenem Offset von -6 000 615 km!
 * Warum veröffentlichen Verbünde keine offenen Daten? (Umfrage)
   * Verbünde haben nicht das Wissen über das Lizenzrecht
   * hätten gerne ein Handbuch zum Thema Open-Data
   * Könnten Anwendungen Dritter die Attraktivität ihres Angebots (Busse und Bahnen) nützen? – Ja
   * Könnten Drittanwendungen Ihnen Geld sparen? – eher Nein
   * Ist das Bereitstellen der Fahrplanauskunft Aufgabe des Verkehrsverbunds/-unternehmens? – stark Ja
   * Sollten Dritte, wenn sie Geld verdienen, auch für die Daten bezahlen? – Ja.
   * Werden die Kunder uns für die falschen Auskünfte Dritter schuldig machen? – starke Ja.
 * Urheberrechtsschutz für Fahrplandaten (als Werk oder Datenbankwerk oder Investitionsschutz)
   * Forschungsbericht Stadtentwicklung
   * Zusammenfassung: vermutlich Nein, bei Rohdaten
   * Aber: Verantwortlichkeit für Korrektheit liegt bei dem Verkehrsverbünde, laut den Verkehrsverbünde.
 * Deutschland != USA
   * Vor vier Jahren wäre die Anwesenheit eines VVSlers undenkbar gewesen.
 * Es geht um GTFS Daten -- also Plane, keine Echtzeitauskünfte
 * Es fehlen intermodale Auskünfte (z.B., mit Car2Go, Bus und Zug).
   * innerdeutsch, bloß ÖPNV geht noch (ohne Preisauskunft), aber nicht international und mehrere Verkehrsmittel

## Diskussionsrunde

 * Deutsche Verkehrswissenschaftliche Gesellschaft
 * Was kriegt man von der DB?
   * Nichts
   * keine Kooperation
 * Wie funktioniert es beii der Bahn selbst?
   * Positionsbestimmung über Blocksignale und Betriebsstellen (Bahnhöfe)
 * Wer scrapet sonst noch?
   * OpenDataCity?? Berlin
   * Openstreetmap scrapt nicht!
 * Problem ist, die gescrapete Daten sind „illegal“
 * Unternehmen denken noch nicht an die Kunden
   * Bahn-Twitter "geht" um 23 Uhr „schlafen“.
   * Da läuft noch die Transformation.
 * Wo sind die Innovationspotentiale aus VVS-Sicht? Ist der Rückkanal Fahrgast → Verbund nicht interessant? (technische Störungen, kaputtes Licht)
 * Echtzeitdaten an Anschlüsse (Bus wartet auf S-Bahn) weitergeben ist ein Projekt des VVS
     * Man ist derzeit „in den letzten Zügen“, dass man langsam von allen Unternehmen die Echtzeitdaten bekommt. Man feilt noch an der Datenqualität. Busfahrer muss noch die Information bekommen.
     * Es wird durchaus vom VVS an so einem System gearbeitet und die Daten werden „demnächst“ ausgeteilt?
 * Man sollte darauf hinarbeiten, dass bei der anstehenden Auschreibung der Regionalzüge in BW die Leistungsbeschreibungen Open-Data-freundlich sind
   * Hinweis auf User locomotive breath auf Drehscheibe-Online
   * über Abgeordnetenwatch sollte man über Andre bei Herrn Verkehrsminister Herrmann
     * Enthalten die Leistungsbeschreibungen zu den Auschreibungen der Regionalverkehre, die Anforderung, dass das Land das Recht erhält, die Solldaten und die Echtverkehrsdaten der betreffenden Regionalverkehre erstens zu erhalten und zweiten als Open-Data in Echtzeit ins Netz zu stellen?
     * http://www.abgeordnetenwatch.de/frage-597-44442--f428392.html#q428392
     * Die Frage wurde von Herrn Schwarz zeitnah - aber leider unvollständig - beantwortet ".. Alle Fragen zur Ausschreibung, zum Betriebskonzept, zum Lastenheft und  zum weiteren Vorgehen finden Sie in der [Landtagsdrucksache 15/5115](http://www.landtag-bw.de/files/live/sites/LTBW/files/dokumente/WP15/Drucksachen/5000/15_5115_D.pdf). .. Einzelne Fragen zu Bekanntgabe der Echtzeitdaten bzw. zum Stand der  Veröffentlichungen der Ausschreibungen beantwortet Ihnen gerne die Nahverkehrsgesellschaft." 
     * Vor einiger Zeit war in der Presse zu lesen, dass das Land ein Förderprogramm für private Busverkehr zur Installation von GPS-Geräten in den Bussen mit dem Ziel, dass das Land mit den Daten, die es gewinnt, eine Verkehrsauskunftsapp erstellt. Stellt das Land die Daten auch als Open-Data ins Netz?
 * Google hätte selbst Performancerobleme, die Echtzeitdaten weltweit live ins Netz zu streamen.
 * Verträge mit dem VVS sagen, Echtzeitdaten durfen für kommerzielle zwecken NICHT weitergegeben werden [also das ist für OpenData auch ein Problem -- die meiste Definitionen erfordern das.]
 * Datenethik
   * Muss also öffentlich sein?
   * Angriffe auf öffentliche Infrastruktur (Terror, Gefahrgutgegner)? – Der Terrorist macht es auch ohne.
   * Datenschutz ist auch ein Thema [sehe auch vorherige session: https://datalove.edupad.uni-konstanz.de/38 ]
 * Katrin Dziekan (Umweltbundesamt)
   * Vor und nach der Einführung der elektronischer Infotafeln an Haltestellen in Oslo
   * gefühlte Verbesserung der Taktdichte, 250.000 Euro Investitionskosten in die Tafeln
 * Mit Open-Data braucht der Verbund nicht jede Station mit einer Tafel ausstatten. Der Dorfladen neben der Haltestelle könnte einen Bildschirm hinters Fenster hängen.
 * Es ist eine Einstellungssache. Wenn die Verbünde den Nutzen erkennen, dann braucht man nicht den Weg über die Politik.
   * HVV (Hamburg) ist weiter/fortschrittlicher (App enthält auch externe Anbieter)
   * VVS bringt demnächst eine intermodale Erweiterung in seiner App
   * Ulm läuft vermutlich etwas hinterher mit intermodale Daten.
 * Werden die Busdaten (GPS) automatisch an die Zentrale gegeben?
   * VVS-System sammelt die Daten (von Busfirmen, DB-RIS, SSB), bündelt sie und verbreitet sie.
   * Beispiel: Abfahrtsmonitor am Milaneo
   * Die meisten Busse haben schon Bordgeräte (Fahrscheindrucker) gehabt, extra Gerät für Echtzeitfähigkeit.
 * Verkehrssteuerung: Werden historische Daten zur Prognose genutzt?
 * VVS-Apps: "Das Stück Google fehlt noch in der App." Die App ist noch nicht intelligent genug bei der Haltestellensuche.
   * Nächste Version hat dieselben Vorzüge wie die Onlinevariante
 * Wünsche
   * Mit offenen Daten kann ich ganz ungewöhnliche Abfragen auch mal machen, da dafür kein wirtschaftilches Interesse machen.
     * Von Aachen nach Düsseldorf Hbf bei GdL-Streik ohne DB Regio: Das geht nicht.
       * EFA-BW (nur BW!) kann's, aber nicht ganz Deutschland
     * möglichst günstig von Ulm nach Frankfurt Flughafen
     * Semesterticket + Länderticket + BC25 + x nach Y
     * VVS sperrt bei SSB-Streik die SSB-Verkehre in der EFA und bietet dann längere Fußwege und Fahrräder an.
   * Warum entwickelt man Apps, wenn es auch schon Google macht und die eigene App das nie so gut hinbekommt?

 * Save the date: `Name fehlt` als Hackday o.ä. zu ÖPNV
 * Empfehlung, die Kooperation mit dem Landesverkehrsministeriums zu suchen, damit es Mitträger einer solchen Veranstaltung wird. Das Ministerium hat einen starken Einfluss, darauf, was mit den Verkehrsdaten der öffentlichen Hand passiert. Es würde bei den wichtigen Leuten das Verständnis für die Anliegen der Community fördern.

Link: http://www.dvwg-wuerttemberg.de/ - DVWG Württemberg e. V.
Hardwareunit zur Standorterfassung der ÖPNV Fahrzeuge: IBIS, Bordgeräte mit Echtzeit

