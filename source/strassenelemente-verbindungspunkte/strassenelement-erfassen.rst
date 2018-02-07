.. index:: Endpunkte, Gesamtstraßennetz, Startpunkte, Straßen, Straßenelemente, Stützpunkte, Topologie, Verbindungspunkte

Straßenelement erfassen
=======================

.. image:: /_static/strassenelement-erfassen.png

.. _strassenelement-erfassen_geometrie:

Geometrie
---------

#. Erfassung des Startpunktes, der Stützpunkte und des Endpunktes (**noch** zu realisieren auf **Applikationsebene**)
#. Prüfung, ob Verbindungspunkte an den Enden vorhanden sind ⇒ automatisierte Erzeugung fehlender Verbindungspunkte (**schon** realisiert auf **Datenbankebene** als Trigger)
#. Herstellung der Anknüpfung des Start- und/oder Endpunktes an das Gesamtstraßennetz (Geometrieanschluss) (**noch** zu realisieren auf **Datenbankebene** ⇒ **noch** zu realisierende Herstellung der Topologie auf **Datenbankebene**, falls möglich)

.. _strassenelement-erfassen_sachdaten:

Sachdaten
---------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen, zum Beispiel mit einer Straße (über diese dann auch Zuordnung der Organisationseinheit, also der zuständigen Verwaltung) und einer Klassifizierung (**noch** zu realisieren auf **Applikationsebene**)
* Eingabe aller verpflichtenden und optionalen Attribute, zum Beispiel einer Bemerkung (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID und der „Ident“ (**schon** realisiert auf **Datenbankebene** über Standardwerte respektive Trigger)
* automatisierte Berechnung der Länge in Metern (**noch** zu realisieren auf **Datenbankebene**)
