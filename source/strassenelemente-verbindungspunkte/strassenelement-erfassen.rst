.. index:: Endpunkte, Gesamtstraßennetz, Startpunkte, Straßen, Straßenelemente, Stützpunkte, Topologie, Verbindungspunkte

Straßenelement erfassen
=======================

.. image:: /_static/strassenelement-erfassen.png

.. _strassenelement-erfassen_geometrie:

Geometrie
---------

#. Erfassung des Startpunktes, der Stützpunkte und des Endpunktes (**Applikationsebene**)
#. Prüfung, ob Verbindungspunkte an den Enden vorhanden sind ⇒ automatisierte Erzeugung fehlender Verbindungspunkte (**Datenbankebene** als Trigger)
#. Herstellung der Anknüpfung des Start- und/oder Endpunktes an das Gesamtstraßennetz (Geometrieanschluss) (**Datenbankebene** als Trigger)

.. _strassenelement-erfassen_sachdaten:

Sachdaten
---------

* Eingabe aller verpflichtenden und optionalen Attribute, zum Beispiel einer Bemerkung (**Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID und der „Ident“ (**Datenbankebene** respektive Trigger)
* automatisierte Berechnung der Länge in Metern (**Datenbankebene** als Trigger)

.. _strassenelement-erfassen_verknuepfungen:

Verknüpfungen
-------------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen, zum Beispiel mit einer Straße (über diese dann auch Zuordnung der Organisationseinheit, also der zuständigen Verwaltung) und einer Klassifizierung (**Applikationsebene**)
