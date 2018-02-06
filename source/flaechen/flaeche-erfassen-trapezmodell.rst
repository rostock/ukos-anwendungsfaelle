.. index:: Flächen, Querprofil, Stationierung, Straßenelemente, Stützpunkte, Teilelemente, Topologie

Fläche mittels Stationierung und Querprofil erfassen („Trapezmodell“)
=====================================================================

.. image:: /_static/flaeche-erfassen-trapezmodell.png

.. _flaeche-erfassen-trapezmodell_geometrie:

Geometrie
---------

#. Erfassung von Straßenelementpunkten und Querprofilen, und zwar nur auf *einem* Straßenelement (also zwischen zwei Verbindungspunkten) (**noch** zu realisieren auf **Applikationsebene**):
    * Erfassung des Start-Straßenelementpunktes oder Auswahl des Start-Verbindungspunktes
    * Erfassung des Ende-Straßenelementpunktes oder Auswahl des Ende-Verbindungspunktes
    * Erfassung der dazwischenliegenden Straßenelementpunkte
    * Eingabe der L- und R-Ordinaten der Querprofile
#. Erzeugung einer Fläche als geschlossenes Polygon (**noch** zu realisieren auf **Applikationsebene**)
#. falls Straßenelementpunkte entstanden sind: Teilelement auf Straßenelement bilden (**noch** zu realisieren auf **Datenbankebene**)
#. falls Straßenelementpunkte entstanden sind: Verknüpfung des Teilelementes und des betroffenen Straßenelementes (Erfüllung der Bedingung 1..1-Verknüpfung zwischen Straßenelement und Fläche) mit der Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. falls keine Straßenelementpunkte entstanden sind: Verknüpfung des betroffenen Straßenelementes (Erfüllung der Bedingung 1..1-Verknüpfung zwischen Straßenelement und Fläche) mit der Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. Prüfung der Topologie (**noch** zu realisieren auf **Datenbankebene**)

**Anmerkung:** Im Resultat ist dieser Anwendungsfall identisch mit dem Anwendungsfall :doc:`../flaechen/flaeche-erfassen-zeichnen`, da in beiden Fällen die Applikationsebene einfach eine Fläche an die Datenbankebene übergibt. Nur die konstruktionsbezogene Herangehensweise auf Applikationsebene ist unterschiedlich. Grundsätzlich gilt: Wurde eine Fläche mittels Stationierung und Querprofil erfasst, soll sie dennoch mittels Zeichnen weiterbearbeitet werden können.


.. _flaeche-erfassen-trapezmodell_sachdaten:

Sachdaten
---------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**noch** zu realisieren auf **Applikationsebene**)
* Eingabe aller verpflichtenden und optionalen Attribute (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**schon** realisiert auf **Datenbankebene** über Standardwerte)
* automatisierte Berechnung des Flächeninhaltes in Quadratmetern (**noch** zu realisieren auf **Datenbankebene**)
