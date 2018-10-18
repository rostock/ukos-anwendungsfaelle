.. index:: Stationierung, Straßenelemente, Strecken, Stützpunkte, Teilelemente

Strecke bearbeiten (Geometrie via Stützpunkte ändern)
=====================================================

.. image:: /_static/strecke-bearbeiten.png

.. _strecke-bearbeiten_geometrie:

Geometrie
---------

#. Verschiebung des Start-Stützpunktes – liefert zugleich auch das (ggf. neue) Start-Straßenelement (**noch** zu realisieren auf **Applikationsebene**)
#. Fällung der Lotrechten auf das betroffene Start-Straßenelement und entsprechende Verschiebung des vorhandenen Start-Straßenelementpunktes (**noch** zu realisieren auf **Datenbankebene**)
#. Verschiebung des Ende-Stützpunktes – liefert zugleich auch das (ggf. neue) Ende-Straßenelement (**noch** zu realisieren auf **Applikationsebene**) (**noch** zu realisieren auf **Applikationsebene**)
#. Fällung der Lotrechten auf das betroffene Ende-Straßenelement und entsprechende Verschiebung des vorhandenen Ende-Straßenelementpunktes (**noch** zu realisieren auf **Datenbankebene**)
#. Teilelement auf Start-Straßenelement (von Start-Straßenelementpunkt bis nächsten Verbindungspunkt in Richtung Ende-Straßenelement) neu bilden (**noch** zu realisieren auf **Datenbankebene**)
#. Teilelement auf Ende-Straßenelement (von nächstem Verbindungspunkt aus Richtung Start-Straßenelement bis Ende-Straßenelementpunkt) neu bilden (**noch** zu realisieren auf **Datenbankebene**)
#. alte Teilelemente löschen
#. Neuberechnung aller zwischen dem Start-Straßenelement und dem Ende-Straßenelement liegenden Straßenelemente unter der Bedingung, dass es nur einen Weg gibt (man also ab dem Start-Straßenelement immer zu genau einem nächsten Straßenelement „springen“ kann, bis man schließlich das Ende-Straßenelement erreicht) (**noch** zu realisieren auf **Datenbankebene**); ansonsten abbrechen mit Hinweis, dass keine eindeutige Strecke ermittelt werden konnte und dass somit die Bearbeitung abgebrochen werden muss (**noch** zu realisieren auf **Applikationsebene**)
#. falls vorheriger Schritt nicht abgebrochen: Neuildung der Strecke durch Neuerknüpfung des Teilelements auf dem Start-Straßenelement, des Teilelements auf dem Ende-Straßenelement und aller dazwischenliegenden Straßenelemente (**noch** zu realisieren auf **Datenbankebene**)

.. _strecke-bearbeiten_sachdaten:

Sachdaten
---------

ohne Änderung

.. _strecke-bearbeiten_verknuepfungen:

Verknüpfungen
-------------

* optionale Anpassung aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**noch** zu realisieren auf **Applikationsebene**)
