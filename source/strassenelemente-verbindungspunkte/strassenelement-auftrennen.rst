.. index:: Endpunkte, Gesamtstraßennetz, Startpunkte, Stationierung, Straßen, Straßenelemente, Straßenelementpunkte, Topologie, Verbindungspunkte

Straßenelement auftrennen (Verbindungspunkt einfügen)
=====================================================

.. image:: /_static/strassenelement-auftrennen.png

.. _strassenelement-auftrennen_geometrie:

Geometrie
---------

#. Auftrennung des vorhandenen Straßenelementes an einem Punkt, das heißt Festlegung des Einfügeortes eines neuen Verbindungspunktes in vorhandene Geometrie eines Straßenelementes (**noch** zu realisieren auf **Applikationsebene**)
#. Teilung des vorhandenen Straßenelementes in zwei neue Straßenelemente und Aktualisierung der zugehörigen Verbindungspunkte (**noch** zu realisieren auf **Datenbankebene**)
#. Herstellung der Anknüpfung des Start- und/oder Endpunktes an das Gesamtstraßennetz (Geometrieanschluss) (**noch** zu realisieren auf **Datenbankebene** ⇒ **noch** zu realisierende Herstellung der Topologie auf **Datenbankebene**, falls möglich)
#. Neuberechnung der Straßenelementpunkte (**noch** zu realisieren auf **Datenbankebene**)

.. _strassenelement-auftrennen_sachdaten:

Sachdaten
---------

* Übernahme oder Neueingabe aller verpflichtenden und optionalen Attribute in/für die beiden neuen Straßenelemente, zum Beispiel einer Bemerkung (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Übernahme aller gemäß Datenbankmodell verpflichtenden Verknüpfungen in die beiden neuen Straßenelemente, zum Beispiel mit einer Straße (über diese dann auch Zuordnung der Organisationseinheit, also der zuständigen Verwaltung) und einer Klassifizierung (**noch** zu realisieren auf **Datenbankebene**)
* automatisierte Aufteilung aller 1..1-Verknüpfungen anderer Objekte mit dem vorhandenen Straßenelement auf die beiden neuen Straßenelemente, und zwar je nach Lage des anderen Objektes zu genau einem der beiden neuen Straßenelemente, sodass nach wie vor 1..1-Verknüpfungen bestehen (**noch** zu realisieren auf **Datenbankebene**)
* automatisierte Übernahme aller weiteren verpflichtenden Attribute in die beiden neuen Straßenelemente *außer* der UUID (**schon** realisiert auf **Datenbankebene** über Standardwerte)
* automatisierte Neuberechnung der Längen in Metern der beiden neuen Straßenelemente (**noch** zu realisieren auf **Datenbankebene**)
