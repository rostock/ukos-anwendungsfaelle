.. index:: Flächen, Querprofil, Stationierung, Straßenelemente, Stützpunkte, Teilelemente, Topologie

Fläche aus Stationierung und Querprofil erzeugen
================================================

.. image:: /_static/flaeche-erzeugen.png

.. _flaeche-erzeugen_geometrie:

Geometrie
---------

#. Erfassung von Straßenelementpunkten und Querprofilen (**noch** zu realisieren auf **Applikationsebene**):
    
    * Erfassung des Start-Straßenelementpunktes und damit zugleich Festlegung des Start-Straßenelements
    * Erfassung des Ende-Straßenelementpunktes und damit zugleich Festlegung des Ende-Straßenelements
    * Erfassung der dazwischenliegenden Straßenelementpunkte für die Querprofile
    * Eingabe der L- und R-Ordinaten der Querprofile an jedem dazwischenliegenden Straßenelementpunkt für die Querprofile

#. Erzeugung einer Fläche als geschlossenes Polygon (**noch** zu realisieren auf **Applikationsebene**)
#. Teilelement auf Start-Straßenelement (von Start-Straßenelementpunkt bis nächsten Verbindungspunkt in Richtung Ende-Straßenelement) bilden (**noch** zu realisieren auf **Datenbankebene**)
#. Teilelement auf Ende-Straßenelement (von nächstem Verbindungspunkt aus Richtung Start-Straßenelement bis Ende-Straßenelementpunkt) bilden (**noch** zu realisieren auf **Datenbankebene**)
#. Verknüpfung der Teilelemente und der dazwischenliegenden Straßenelemente mit der Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. Prüfung der Topologie (**noch** zu realisieren auf **Datenbankebene**)


.. _flaeche-erzeugen_sachdaten:

Sachdaten
---------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**noch** zu realisieren auf **Applikationsebene**)
* Eingabe aller verpflichtenden und optionalen Attribute (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**schon** realisiert auf **Datenbankebene** über Standardwerte)
* automatisierte Berechnung des Flächeninhaltes in Quadratmetern (**noch** zu realisieren auf **Datenbankebene**)
