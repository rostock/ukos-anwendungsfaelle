.. index:: Stationierung, Straßenelemente, Strecken, Stützpunkte, Teilelemente

Strecke erfassen
================

.. image:: /_static/strecke-erfassen.png

.. _strecke-erfassen_geometrie:

Geometrie
---------

#. Erfassung des Start-Stützpunktes – liefert zugleich auch Start-Straßenelement (**noch** zu realisieren auf **Applikationsebene**)
#. Fällung der Lotrechten auf das betroffene Start-Straßenelement zur Ermittlung des Start-Straßenelementpunktes (**noch** zu realisieren auf **Datenbankebene**)
#. Erfassung des Ende-Stützpunktes – liefert zugleich auch Ende-Straßenelement (**noch** zu realisieren auf **Applikationsebene**)
#. Fällung der Lotrechten auf das betroffene Ende-Straßenelement zur Ermittlung des Ende-Straßenelementpunktes (**noch** zu realisieren auf **Datenbankebene**)
#. Teilelement auf Start-Straßenelement (von Start-Straßenelementpunkt bis nächsten Verbindungspunkt in Richtung Ende-Straßenelement) bilden (**noch** zu realisieren auf **Datenbankebene**)
#. Teilelement auf Ende-Straßenelement (von nächstem Verbindungspunkt aus Richtung Start-Straßenelement bis Ende-Straßenelementpunkt) bilden (**noch** zu realisieren auf **Datenbankebene**)
#. Berechnung aller zwischen dem Start-Straßenelement und dem Ende-Straßenelement liegenden Straßenelemente unter der Bedingung, dass es nur einen Weg gibt (man also ab dem Start-Straßenelement immer zu genau einem nächsten Straßenelement „springen“ kann, bis man schließlich das Ende-Straßenelement erreicht) (**noch** zu realisieren auf **Datenbankebene**); ansonsten abbrechen mit Hinweis, dass keine eindeutige Strecke ermittelt werden konnte und dass somit mehrere separate Strecken gebildet werden müssen (**noch** zu realisieren auf **Applikationsebene**)
#. falls vorheriger Schritt nicht abgebrochen: Bildung der Strecke durch Verknüpfung des Teilelements auf dem Start-Straßenelement, des Teilelements auf dem Ende-Straßenelement und aller dazwischenliegenden Straßenelemente (**noch** zu realisieren auf **Datenbankebene**)

.. _strecke-erfassen_sachdaten:

Sachdaten
---------

* Eingabe aller verpflichtenden und optionalen Attribute, zum Beispiel einer Bemerkung (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**schon** realisiert auf **Datenbankebene** über Standardwerte)
* automatisierte Berechnung der Länge in Metern (**noch** zu realisieren auf **Datenbankebene**)

.. _strecke-erfassen_verknuepfungen:

Verknüpfungen
-------------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen, zum Beispiel mit einer Straße (über diese dann auch Zuordnung der Organisationseinheit, also der zuständigen Verwaltung) und einer Klassifizierung (**noch** zu realisieren auf **Applikationsebene**)
