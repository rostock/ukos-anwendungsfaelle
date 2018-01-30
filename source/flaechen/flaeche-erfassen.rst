.. index:: Flächen, Stationierung, Straßenelemente, Stützpunkte, Teilelemente, Topologie

Fläche erfassen
===============

.. image:: /_static/flaeche-erfassen.png

.. _flaeche-erfassen_geometrie:

Geometrie
---------

#. Erfassung einer Fläche als geschlossenes Polygon durch Erfassung von Stützpunkten (**noch** zu realisieren auf **Applikationsebene**)
#. Erstellung von Straßenelementpunkten überall dort, wo die Fläche Straßenelemente schneidet (**noch** zu realisieren auf **Datenbankebene**)
#. Teilelement auf Start-Straßenelement (von Start-Straßenelementpunkt bis nächsten Verbindungspunkt in Richtung Ende-Straßenelement) bilden: Start-Straßenelement ist hier jenes Straßenelement, das „links“ keine weiteren Straßenelemente mit durch die Flächenverschneidung entstandenen Straßenelementpunkten mehr aufweist (**noch** zu realisieren auf **Datenbankebene**)
#. Teilelement auf Ende-Straßenelement (von nächstem Verbindungspunkt aus Richtung Start-Straßenelement bis Ende-Straßenelementpunkt) bilden: Ende-Straßenelement ist hier jenes Straßenelement, das „rechts“ keine weiteren Straßenelemente mit durch die Flächenverschneidung entstandenen Straßenelementpunkten mehr aufweist (**noch** zu realisieren auf **Datenbankebene**)
#. Verknüpfung der Teilelemente und der dazwischenliegenden Straßenelemente mit der Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. Prüfung der Topologie (**noch** zu realisieren auf **Datenbankebene**)

.. _flaeche-erfassen_sachdaten:

Sachdaten
---------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**noch** zu realisieren auf **Applikationsebene**)
* Eingabe aller verpflichtenden und optionalen Attribute (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**schon** realisiert auf **Datenbankebene** über Standardwerte)
* automatisierte Berechnung des Flächeninhaltes in Quadratmetern (**noch** zu realisieren auf **Datenbankebene**)
