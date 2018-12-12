.. index:: Endpunkte, Gesamtstraßennetz, Startpunkte, Stationierung, Straßen, Straßenelemente, Straßenelementpunkte, Topologie, Verbindungspunkte

Straßenelement auftrennen (Verbindungspunkt einfügen)
=====================================================

.. image:: /_static/strassenelement-auftrennen.png

.. _strassenelement-auftrennen_geometrie:

Geometrie
---------

#. Auftrennung des vorhandenen Straßenelementes an einem Punkt, das heißt Festlegung des Einfügeortes eines neuen Verbindungspunktes in vorhandene Geometrie eines Straßenelementes (**Applikationsebene**)
#. Teilung des vorhandenen Straßenelementes in zwei neue Straßenelemente (**Applikationsebene**)
#. Aktualisierung der zugehörigen Verbindungspunkte (**Datenbankebene**)

.. _strassenelement-auftrennen_sachdaten:

Sachdaten
---------

* Übernahme oder Neueingabe aller verpflichtenden und optionalen Attribute in/für die beiden neuen Straßenelemente, zum Beispiel einer Bemerkung (**Applikationsebene**)
* automatisierte Übernahme aller weiteren verpflichtenden Attribute in die beiden neuen Straßenelemente *außer* der UUID und der „Ident“, die jeweils neu erstellt werden (**Datenbankebene** respektive Trigger)
* automatisierte Neuberechnung der Längen in Metern der beiden neuen Straßenelemente (**Datenbankebene**)

.. _strassenelement-auftrennen_verknuepfungen:

Verknüpfungen
-------------

* automatisierte Übernahme aller gemäß Datenbankmodell verpflichtenden Verknüpfungen in die beiden neuen Straßenelemente, zum Beispiel mit einer Straße (über diese dann auch Zuordnung der Organisationseinheit, also der zuständigen Verwaltung) und einer Klassifizierung (**Datenbankebene**)
* automatisierte Aufteilung der Verknüpfungen aller Straßenelementpunkte und anderer Objekte mit dem ehemals vorhandenen Straßenelement auf die beiden neuen Straßenelemente, und zwar je nach Lage des Straßenelementpunktes oder anderen Objektes zu genau einem der beiden neuen Straßenelemente, sodass nach wie vor Verknüpfungen bestehen (**Datenbankebene**)
