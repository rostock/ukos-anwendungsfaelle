.. index:: Stationierung, Straßenelemente, Strecken, Stützpunkte, Teilelemente

Strecke erfassen
================

.. image:: /_static/strecke-erfassen.png

.. _strecke-erfassen_geometrie:

Geometrie
---------

#. Erfassung des Start-Straßenelementpunktes – liefert zugleich auch Start-Straßenelement (**Applikationsebene**)
#. Erfassung des Ende-Straßenelementpunktes – liefert zugleich auch Ende-Straßenelement (**Applikationsebene**)
#. Teilelement auf Start-Straßenelement (von Start-Straßenelementpunkt bis nächsten Verbindungspunkt in Richtung Ende-Straßenelement) bilden (**Datenbankebene**)
#. Teilelement auf Ende-Straßenelement (von nächstem Verbindungspunkt aus Richtung Start-Straßenelement bis Ende-Straßenelementpunkt) bilden (**Datenbankebene**)
#. Berechnung aller zwischen dem Start-Straßenelement und dem Ende-Straßenelement liegenden Teilelemente (die hier dann den Straßenelementen entsprechen) unter der Bedingung, dass es nur einen Weg gibt (man also ab dem Start-Straßenelement immer zu genau einem nächsten Straßenelement „springen“ kann, bis man schließlich das Ende-Straßenelement erreicht) (**Datenbankebene**); ansonsten abbrechen mit Hinweis, dass keine eindeutige Strecke ermittelt werden konnte und dass somit mehrere separate Strecken gebildet werden müssen (**Applikationsebene**)
#. falls vorheriger Schritt nicht abgebrochen: Bildung der Strecke durch Verknüpfung des Teilelements auf dem Start-Straßenelement, des Teilelements auf dem Ende-Straßenelement und aller dazwischenliegenden Teilelemente (**Datenbankebene**)

.. _strecke-erfassen_sachdaten:

Sachdaten
---------

* Eingabe aller verpflichtenden und optionalen Attribute, zum Beispiel einer Bemerkung (**Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**Datenbankebene**)
* automatisierte Berechnung der Länge in Metern (**Datenbankebene**)

.. _strecke-erfassen_verknuepfungen:

Verknüpfungen
-------------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen, zum Beispiel mit einer Straße (über diese dann auch Zuordnung der Organisationseinheit, also der zuständigen Verwaltung) und einer Klassifizierung (**Applikationsebene**)
