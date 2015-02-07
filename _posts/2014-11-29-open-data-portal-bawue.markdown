---
layout: post_14
title:  "Open Data Portal Baden-Württemberg"
author: Stephan Jaud
category: 14
---

 * Die URL wird noch nicht veröffentlicht, da die Abnahme noch nicht erfolgt ist, noch pre-Alpha und noch nicht bezahlt.
 * momentan nur Testdaten

<figure>
  <a href="https://www.flickr.com/photos/okfde/15817777970" title="OpenCityCamp Stuttgart 2014 by Open Knowledge Foundation Deutschland, on Flickr"><img src="https://farm8.staticflickr.com/7532/15817777970_214f0bb3bd_z.jpg" width="640" height="427" alt="OpenCityCamp Stuttgart 2014"></a>
<figcaption>
  Bild <a href="https://creativecommons.org/licenses/by/2.0/">CC-BY</a> Awesome Pixels.
</figcaption>
</figure>


## Was soll ins Portal?


 * Erschließen der VVS-GTFS-Daten über dieses Portal
 * Landesverwaltung  hat schon viele viele Daten veröffentlicht, aber verstreut und  unsortiert und meist gut versteckt (z.T. nicht über Google auffindbar).
 * Hauptziel: Über eine Adresse soll anhand von Metadaten gesucht und gefunden werden.
 * Nebenziel: standardisierte Bereitstellung, Formate und Nutzungsbedingungen

## Govdata

 * Jaud ist Vertreter von BW in der Bund-Länder-Arbeitsgruppe zum Govdata-Portal.
 * Govdata wird ab 2015 als Portal weiter am Leben bleiben.
 * Nicht ein großes, zentrales Portal, sondern viele Portale. Ansonsten 10.000 Datenbereitsteller und eine riesige Redaktion.
 * Daher Landesportale bei Flächenländern nach Govdata-Standard, Metadatenaustausch über festgelegte Schnittstellen.
 * Aufnahme städtischer Daten

## Lizenzen

 * Man hat sich gegen CC- und für selbstgemachte Lizenz ([Datenlizenz Deutschland](https://www.govdata.de/lizenzen)) entschieden und verkündet das als Empfehlung der Bund-Länder-Arbeitsgruppe.
   * Man wollte einen kurzen Lizenztext. CC sei zu lange (langatmig wie bei Apple & Co.)
 * kurze Erläuterung von Datenlizenz DE 1.0 und 2.0
 * manche Kritiker auf Verwaltungsseite würden Haftungsregelungen gerne aufnehmen
   * Man kommt als Staat nicht aus der Staatshaftung heraus.

## Das Portal

 * [Vorgänger](http://opendata.service-bw.de) war Prototyp und nur zum Testen, aber mit echten Daten
 * mittlerweile neues Konzept, das sich an Govdata anlehnt
 * in der Grundstufe ist so ein Portal nur wenig komplex
 * Nicht  nur stark IT-affine Personen sollten das Portal nutzen können. Wer  schon mal ein bisschen im Internet unterwegs war sollte es nutzen können.
 * Wenn die Leute nicht gezielt suchen, dann suchen sie über ihren Wohnort → daher kartenbasierte Suchfunktion
 * Zum Bewerten von Datensätzen muss man sich einloggen. Registrierung auf „niedrigem Vertrauensniveau“.

Feedbackrunde
-------------

 * Gemeinde (Breadcumb) könnte größer dargestellt werden oder als "Kärtchen" unter dem Datensatz
 * Was macht die Vorschau?
   * noch nichts bei Einwohner in Ochsenhausen
   * funktioniert bei Schulen im Kreis Biberach
 * „Ich habe gerade wieder zwei weitere Fehler gefunden.“
 * Warum sind es in BW nur 12, auf Govdata 14 Kategorien?
   * eigener Kategorienkatalog, der an Bund angelehnt ist
   * Umweltministerium wollte das Thema Energien in den Kategorien haben, was bundesweit nicht durchsetzbar war
 * Wenn man Nicht-Standardlizenzen verwendet, sollte man eine  Kompatibilitätsliste anbieten. Dann können juristisch wenig bewanderte Entwickler das leichter herausfinden.
   * Datenlizenz DE [ist als Open anerkannt im Sinne der Open-Definition](http://okfn.de/2014/09/erfolg-fuer-open-data-datenlizenz-deutschland-version-2-0-ist-eine-offene-lizenz/)
   * Kategorien anbieten: kommerziell erlaubt, kommerzielle Weitergabe erlaubt, Share-Alike, … (wie das CC-Logo)
   * als Filter in der Suche
 * CC-Lizenzen werden ohne Versionsnummer angegeben
 * Art und Weise der Namensnennung muss noch ergänzt werden als Datenfeld in der Metadatenbank
 * Beschreibungen der Kategorien in Vorschautabellen (z.B. bei CSV-Daten)
   * Wir möchten möglichst wenig erklären.
   * "Politik und Verwaltung" ist schwer zu erklären.
   * Daten sind aufbereitet durch die Nutzung durch Fachleute.
   * Metadaten und Kurzbeschreibungstexte sind von Fachleuten für Fachleute beschrieben.
   * Das ist das Problem, das Verwaltungen haben, wenn sie plötzlich Daten öffentlich bereitstellen.
   * Ämter haben keine Zeit (Personal), lange Beschreibungen zu schreiben und daher sind die Beschreibungen kurz, da man sonst keine Daten bekommt.
   * 1879 war die erste Konferenz zur Standardisierung statistischer Daten.
     * Das kann man nicht anordnen und zwingen, da der Staat sonst es bezahlen müsste.
   * Daher erst die Daten ins Netz kippen.
   * Anregungen: Datenbeschreibung könnte man als Wiki machen, denn "Open" heißt auch "Mitmachen":
   * Datenfehler melden
     * Kommentare an den Datensätzen sind eingeloggt möglich und werden nichtöffentlich an die Behörde weitergeleitet.
     * Das sollte "Feedback" oder "Fehler melden" und nicht "Kommentar" nennen.
 * Filter direkt verlinken und branden, damit ein Landkreis auf seinen Teil im Portal verlinken kann ("Unsere Datensätze")
   * wird ab 2016 als Datenportal des Landes (und der Kommunen) als service-bw.de vermarktet
   * [service-bw.de](http://www.service-bw.de) wurde gerade neu ausgeschrieben und beitet Kommunen die Möglichkeit, Teile des Portals zu sich zu übernehmen
 * Datenwunschfunktion gibt es nicht
 * Datennutzungsmeldungsfunktion als Rückmeldung
 * Bei Schnittstellen wäre eine Unterstützungsgarantie und eine "Kündigungsfrist" von Seiten des Datenbereitstellers nett.

## Welche Daten kommen da hin?

 * Angst der Community vor Mehrfachveröffentlichung unter verschiedenen Lizenzen
   * Govdata und andere Portale verlinken nur auf die Quelle
   * zusätzlicher Erschließungsweg zu Fachportalen
 * Die statistischen Daten haben derzeit schon mehr Standards und kann daher mehr Datensätze zur Verfügung stellen als anderer Bereiche.
 * Datenhistorie
   * Was die Gemeinde reinstellt, geht rein.
   * Es gibt statiste Daten und dynamische Daten.


 * In der vorherigen Version des Portals gibt es noch Haushaltsplandaten von 2007 bis 2014


