.. index:: Flächen, Stationierung, Straßenelemente, Stützpunkte, Teilelemente, Topologie

Fläche mittels Zeichnen erfassen
================================

.. image:: /_static/flaeche-erfassen-zeichnen.png

.. _flaeche-erfassen-zeichnen_geometrie:

Geometrie
---------

#. Erfassung einer Fläche als geschlossenes Polygon durch Erfassung von Stützpunkten, und zwar nur auf *einem* Straßenelement (also zwischen zwei Verbindungspunkten) (**Applikationsebene**)
#. Erstellung von Straßenelementpunkten überall dort, wo die Fläche das Straßenelement schneidet und dabei *nicht* durch einen Verbindungspunkt geht (**Datenbankebene**)
#. falls Straßenelementpunkte entstanden sind: Teilelement auf Straßenelement bilden (**Datenbankebene**)
#. falls Straßenelementpunkte entstanden sind: Verknüpfung des Teilelementes, der Straßenelementpunkte und des betroffenen Straßenelementes mit der Fläche – Erfüllung der Bedingung der Verknüpfung zwischen Straßenelement und Fläche (**Datenbankebene**)
#. falls keine Straßenelementpunkte entstanden sind: Verknüpfung des betroffenen Straßenelementes mit der Fläche – Erfüllung der Bedingung der Verknüpfung zwischen Straßenelement und Fläche (**Datenbankebene**)
#. Prüfung der Topologie (**Datenbankebene**)

**Anmerkung:** Im Resultat ist dieser Anwendungsfall identisch mit dem Anwendungsfall :doc:`../flaechen/flaeche-erfassen-trapezmodell`, da in beiden Fällen die Applikationsebene einfach ein Flächen an die Datenbankebene übergibt. Nur die konstruktionsbezogene Herangehensweise auf Applikationsebene ist unterschiedlich. Grundsätzlich gilt: Wurde eine Fläche mittels Zeichnen erfasst, soll sie dennoch mittels Stationierung und Querprofil weiterbearbeitet werden können.

.. _flaeche-erfassen-zeichnen_sachdaten:

Sachdaten
---------

* Eingabe aller verpflichtenden und optionalen Attribute (**Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**Datenbankebene**)
* automatisierte Berechnung des Flächeninhaltes in Quadratmetern (**Datenbankebene**)

.. _flaeche-erfassen-zeichnen_verknuepfungen:

Verknüpfungen
-------------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**Applikationsebene**)
