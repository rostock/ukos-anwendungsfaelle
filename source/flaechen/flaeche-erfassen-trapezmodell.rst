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
    * Eingabe aller L- und R-Ordinaten der Querprofile
#. Erzeugung der Querschnittsflächen als einzelne, geschlossene Polygone (**noch** zu realisieren auf **Applikationsebene**)
#. falls Straßenelementpunkte entstanden sind: Teilelemente auf Straßenelement bilden (**noch** zu realisieren auf **Datenbankebene**)
#. falls Straßenelementpunkte entstanden sind: Verknüpfung der Teilelemente, der Straßenelementpunkte und des betroffenen Straßenelementes mit jeweils passender Querschnittsfläche – Erfüllung der Bedingung der Verknüpfung zwischen Straßenelement und Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. falls keine Straßenelementpunkte entstanden sind: Verknüpfung des betroffenen Straßenelementes mit der Querschnittsfläche – Erfüllung der Bedingung der Verknüpfung zwischen Straßenelement und Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. Prüfung der Topologie (**noch** zu realisieren auf **Datenbankebene**)
#. Erzeugung der übergeordneten Verkehrsfläche und Verknüpfung der Querschnittsfläche(n) mit dieser (**noch** zu realisieren auf **Datenbankebene**)

**Anmerkung:** Im Resultat ist dieser Anwendungsfall identisch mit dem Anwendungsfall :doc:`../flaechen/flaeche-erfassen-zeichnen`, da in beiden Fällen die Applikationsebene einfach Flächen an die Datenbankebene übergibt. Nur die konstruktionsbezogene Herangehensweise auf Applikationsebene ist unterschiedlich. Grundsätzlich gilt: Wurde eine Fläche mittels Stationierung und Querprofil erfasst, soll sie dennoch mittels Zeichnen weiterbearbeitet werden können.


.. _flaeche-erfassen-trapezmodell_sachdaten:

Sachdaten
---------

* Eingabe aller verpflichtenden und optionalen Attribute (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**schon** realisiert auf **Datenbankebene** über Standardwerte)
* automatisierte Berechnung des Flächeninhaltes in Quadratmetern (**noch** zu realisieren auf **Datenbankebene**)

.. _flaeche-erfassen-trapezmodell_verknuepfungen:

Verknüpfungen
-------------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**noch** zu realisieren auf **Applikationsebene**)
