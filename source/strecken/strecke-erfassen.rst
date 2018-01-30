.. index:: Stationierung, Straßenelemente, Strecken, Stützpunkte, Teilelemente

Strecke erfassen
================

.. image:: /_static/strecke-erfassen.png

.. _strecke-erfassen_geometrie:

Geometrie
---------

#. Erfassung des Start-Stützpunktes (**noch** zu realisieren auf **Applikationsebene**)
#. Auswahl des betroffenen Start-Straßenelements (**noch** zu realisieren auf **Applikationsebene**)
#. Fällung der Lotrechten auf das betroffene Start-Straßenelement zur Ermittlung des Start-Straßenelementpunktes (**noch** zu realisieren auf **Datenbankebene**)
#. Erfassung des Ende-Stützpunktes (**noch** zu realisieren auf **Applikationsebene**)
#. Auswahl des betroffenen Ende-Straßenelements (**noch** zu realisieren auf **Applikationsebene**)
#. Fällung der Lotrechten auf das betroffene Ende-Straßenelement zur Ermittlung des Ende-Straßenelementpunktes (**noch** zu realisieren auf **Datenbankebene**)
#. Teilelement auf Start-Straßenelement (von Start-Straßenelementpunkt bis nächsten Verbindungspunkt in Richtung Ende-Straßenelement) bilden (**noch** zu realisieren auf **Datenbankebene**)
#. Teilelement auf Ende-Straßenelement (von nächstem Verbindungspunkt aus Richtung Start-Straßenelement bis Ende-Straßenelementpunkt) bilden (**noch** zu realisieren auf **Datenbankebene**)
#. Verknüpfung der Teilelemente und der dazwischenliegenden Straßenelemente mit der Strecke (**noch** zu realisieren auf **Datenbankebene**)

.. _strecke-erfassen_sachdaten:

Sachdaten
---------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen, zum Beispiel mit einer Straße (über diese dann auch Zuordnung der Organisationseinheit, also der zuständigen Verwaltung) und einer Klassifizierung (**noch** zu realisieren auf **Applikationsebene**)
* Eingabe aller verpflichtenden und optionalen Attribute, zum Beispiel einer Bemerkung (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**schon** realisiert auf **Datenbankebene** über Standardwerte)
* automatisierte Berechnung der Länge in Metern (**noch** zu realisieren auf **Datenbankebene**)
