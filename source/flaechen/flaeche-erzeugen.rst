.. index:: Querprofil, Stationierung, Straßenelemente, Flächen, Stützpunkte, Topologie

Fläche aus Stationierung und Querprofil erzeugen
================================================

.. image:: /_static/flaeche-erzeugen.png

.. _flaeche-erzeugen_geometrie:

Geometrie
---------

#. Erfassung von Straßenelementpunkten und Querprofilen (**noch** zu realisieren auf **Applikationsebene**):
    
    * Erfassung des Start-Straßenelementpunktes
    * Erfassung der Straßenelementpunktes für die Querprofile
    * Erfassung des Ende-Straßenelementpunktes
    * Eingabe der L- und R-Ordinaten der Querprofile

#. Erzeugung einer Fläche als geschlossenes Polygon (**noch** zu realisieren auf **Applikationsebene**)
#. Prüfung der Topologie (**noch** zu realisieren auf **Datenbankebene**)


.. _flaeche-erzeugen_sachdaten:

Sachdaten
---------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**noch** zu realisieren auf **Applikationsebene**)
* Eingabe aller verpflichtenden und optionalen Attribute (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**schon** realisiert auf **Datenbankebene** über Standardwerte)
* automatisierte Berechnung des Flächeninhaltes in Quadratmetern (**noch** zu realisieren auf **Datenbankebene**)
