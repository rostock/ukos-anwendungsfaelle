.. index:: Stationierung, Straßenelemente, Strecken, Stützpunkte, Teilelemente

Strecke bearbeiten (Geometrie via Stützpunkte ändern)
=====================================================

.. image:: /_static/strecke-bearbeiten.png

.. _strecke-bearbeiten_geometrie:

Geometrie
---------

#. Verschiebung des Start-Straßenelementpunktes – liefert zugleich auch das (ggf. neue) Start-Straßenelement (**Applikationsebene**)
#. Verschiebung des Ende-Straßenelementpunktes – liefert zugleich auch das (ggf. neue) Ende-Straßenelement (**Applikationsebene**)
#. Teilelement auf Start-Straßenelement (von Start-Straßenelementpunkt bis nächsten Verbindungspunkt in Richtung Ende-Straßenelement) neu bilden (**Datenbankebene**)
#. Teilelement auf Ende-Straßenelement (von nächstem Verbindungspunkt aus Richtung Start-Straßenelement bis Ende-Straßenelementpunkt) neu bilden (**Datenbankebene**)
#. alte Teilelemente löschen (**Datenbankebene**)
#. Neuberechnung aller zwischen dem Start-Straßenelement und dem Ende-Straßenelement liegenden Teilelemente (die hier dann den Straßenelementen entsprechen) unter der Bedingung, dass es nur einen Weg gibt (man also ab dem Start-Straßenelement immer zu genau einem nächsten Straßenelement „springen“ kann, bis man schließlich das Ende-Straßenelement erreicht) (**Datenbankebene**); ansonsten abbrechen mit Hinweis, dass keine eindeutige Strecke ermittelt werden konnte und dass somit die Bearbeitung abgebrochen werden muss (**Applikationsebene**)
#. falls vorheriger Schritt nicht abgebrochen: Neuildung der Strecke durch Neuerknüpfung des Teilelements auf dem Start-Straßenelement, des Teilelements auf dem Ende-Straßenelement und aller dazwischenliegenden Teilelemente (**Datenbankebene**)

.. _strecke-bearbeiten_sachdaten:

Sachdaten
---------

ohne Änderung

.. _strecke-bearbeiten_verknuepfungen:

Verknüpfungen
-------------

* optionale Anpassung aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**Applikationsebene**)
