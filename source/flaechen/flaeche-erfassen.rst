.. index:: Stationierung, Straßenelemente, Flächen, Stützpunkte, Topologie

Fläche erfassen
===============

.. image:: /_static/flaeche-erfassen.png

.. _flaeche-erfassen_geometrie:

Geometrie
---------

#. Erfassung einer Flächen als geschlossenes Polygon (**noch** zu realisieren auf **Applikationsebene**)
#. Erstellung von Straßenelementpunkten überall dort, wo die Fläche Straßenelemente schneidet (**noch** zu realisieren auf **Datenbankebene**)
#. Prüfung der Topologie (**noch** zu realisieren auf **Datenbankebene**)

.. _flaeche-erfassen_sachdaten:

Sachdaten
---------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**noch** zu realisieren auf **Applikationsebene**)
* Eingabe aller verpflichtenden und optionalen Attribute (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**schon** realisiert auf **Datenbankebene** über Standardwerte)
* automatisierte Berechnung des Flächeninhaltes in Quadratmetern (**noch** zu realisieren auf **Datenbankebene**)
