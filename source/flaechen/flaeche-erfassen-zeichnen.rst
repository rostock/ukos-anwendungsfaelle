.. index:: Flächen, Stationierung, Straßenelemente, Stützpunkte, Teilelemente, Topologie

Fläche mittels Zeichnen erfassen
================================

.. image:: /_static/flaeche-erfassen-zeichnen.png

.. _flaeche-erfassen-zeichnen_geometrie:

Geometrie
---------

#. Erfassung einer Fläche als geschlossenes Polygon durch Erfassung von Stützpunkten, und zwar nur auf *einem* Straßenelement (also zwischen zwei Verbindungspunkten) (**noch** zu realisieren auf **Applikationsebene**)
#. Erstellung von Straßenelementpunkten überall dort, wo die Fläche das Straßenelement schneidet und dabei *nicht* durch einen Verbindungspunkt geht (**noch** zu realisieren auf **Datenbankebene**)
#. falls Straßenelementpunkte entstanden sind: Teilelement auf Straßenelement bilden (**noch** zu realisieren auf **Datenbankebene**)
#. falls Straßenelementpunkte entstanden sind: Verknüpfung des Teilelementes, der Straßenelementpunkte und des betroffenen Straßenelementes mit der Fläche – Erfüllung der Bedingung der Verknüpfung zwischen Straßenelement und Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. falls keine Straßenelementpunkte entstanden sind: Verknüpfung des betroffenen Straßenelementes mit der Fläche – Erfüllung der Bedingung der Verknüpfung zwischen Straßenelement und Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. Prüfung der Topologie (**noch** zu realisieren auf **Datenbankebene**)

**Anmerkung:** Im Resultat ist dieser Anwendungsfall identisch mit dem Anwendungsfall :doc:`../flaechen/flaeche-erfassen-trapezmodell`, da in beiden Fällen die Applikationsebene einfach eine Fläche an die Datenbankebene übergibt. Nur die konstruktionsbezogene Herangehensweise auf Applikationsebene ist unterschiedlich. Grundsätzlich gilt: Wurde eine Fläche mittels Zeichnen erfasst, soll sie dennoch mittels Stationierung und Querprofil weiterbearbeitet werden können.

.. _flaeche-erfassen-zeichnen_sachdaten:

Sachdaten
---------

* Eingabe aller verpflichtenden und optionalen Attribute (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**schon** realisiert auf **Datenbankebene** über Standardwerte)
* automatisierte Berechnung des Flächeninhaltes in Quadratmetern (**noch** zu realisieren auf **Datenbankebene**)

.. _flaeche-erfassen-zeichnen_verknuepfungen:

Verknüpfungen
-------------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**noch** zu realisieren auf **Applikationsebene**)
