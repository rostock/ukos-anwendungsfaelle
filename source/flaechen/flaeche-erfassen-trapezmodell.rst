.. index:: Flächen, Querprofil, Stationierung, Straßenelemente, Stützpunkte, Teilelemente, Topologie

Fläche mittels Stationierung und Querprofil erfassen („Trapezmodell“)
=====================================================================

.. image:: /_static/flaeche-erfassen-trapezmodell.png

.. _flaeche-erfassen-trapezmodell_geometrie:

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

**Anmerkung:** Im Resultat ist dieser Anwendungsfall identisch mit dem Anwendungsfall :doc:`../flaechen/flaeche-erfassen-zeichnen`, da in beiden Fällen die Applikationsebene einfach eine Fläche an die Datenbankebene übergibt. Nur die konstruktionsbezogene Herangehensweise auf Applikationsebene ist unterschiedlich. Grundsätzlich gilt: Wurde eine Fläche mittels Stationierung und Querprofil erfasst, soll sie dennoch mittels Zeichnen weiterbearbeitet werden können.


.. _flaeche-erfassen-trapezmodell_sachdaten:

Sachdaten
---------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**noch** zu realisieren auf **Applikationsebene**)
* Eingabe aller verpflichtenden und optionalen Attribute (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**schon** realisiert auf **Datenbankebene** über Standardwerte)
* automatisierte Berechnung des Flächeninhaltes in Quadratmetern (**noch** zu realisieren auf **Datenbankebene**)
