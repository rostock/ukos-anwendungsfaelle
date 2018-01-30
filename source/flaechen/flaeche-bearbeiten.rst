.. index:: Flächen, Stationierung, Straßenelemente, Stützpunkte, Teilelemente, Topologie

Fläche bearbeiten (Geometrie ändern)
====================================

.. image:: /_static/flaeche-bearbeiten.png

.. _flaeche-bearbeiten_geometrie:

Geometrie
---------

#. Verschiebung der Stützpunkte einer Fläche als geschlossenes Polygon (**noch** zu realisieren auf **Applikationsebene**)
#. Anpassung der Straßenelementpunkte überall dort, wo die Fläche Straßenelemente schneidet (**noch** zu realisieren auf **Datenbankebene**)
#. Teilelement auf Start-Straßenelement (von Start-Straßenelementpunkt bis nächsten Verbindungspunkt in Richtung Ende-Straßenelement) neu bilden – Start-Straßenelement ist hier jenes Straßenelement, das „links“ keine weiteren Straßenelemente mit durch die Flächenverschneidung entstandenen Straßenelementpunkten mehr aufweist (**noch** zu realisieren auf **Datenbankebene**)
#. Teilelement auf Ende-Straßenelement (von nächstem Verbindungspunkt aus Richtung Start-Straßenelement bis Ende-Straßenelementpunkt) neu bilden – Ende-Straßenelement ist hier jenes Straßenelement, das „rechts“ keine weiteren Straßenelemente mit durch die Flächenverschneidung entstandenen Straßenelementpunkten mehr aufweist (**noch** zu realisieren auf **Datenbankebene**)
#. alte Teilelemente löschen
#. Neuverknüpfung der Teilelemente und der dazwischenliegenden Straßenelemente mit der Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. Prüfung der Topologie (**noch** zu realisieren auf **Datenbankebene**)

.. _flaeche-bearbeiten_sachdaten:

Sachdaten
---------

* automatisierte Neuberechnung des Flächeninhaltes in Quadratmetern (**noch** zu realisieren auf **Datenbankebene**)
