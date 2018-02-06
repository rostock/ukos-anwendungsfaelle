.. index:: Flächen, Stationierung, Straßenelemente, Stützpunkte, Teilelemente, Topologie

Fläche mittels Zeichnen erfassen
================================

.. image:: /_static/flaeche-erfassen-zeichnen.png

.. _flaeche-erfassen-zeichnen_geometrie:

Geometrie
---------

#. Erfassung einer Fläche als geschlossenes Polygon durch Erfassung von Stützpunkten (**noch** zu realisieren auf **Applikationsebene**)
#. Erstellung von Straßenelementpunkten überall dort, wo die Fläche Straßenelemente schneidet (**noch** zu realisieren auf **Datenbankebene**)
#. falls Fläche über einen oder mehrere Verbindungspunkte hinausgeht: Auftrennung der Fläche an jedem dieser Verbindungspunkte (jeweilige Auftrennungskante beginnt „links“ in jenem Punkt auf der Flächenaußenkante, der die kürzeste Entfernung zum Verbindungspunkt aufweist, geht durch den Verbindungspunkt und endet „rechts“ in jenem Punkt auf der Flächenaußenkante, der die kürzeste Entfernung zum Verbindungspunkt aufweist) (**noch** zu realisieren auf **Datenbankebene**)
#. falls Fläche aufgetrennt wurde und Straßenelementpunkte entstanden sind: Teilelemente auf Straßenelementen bilden (**noch** zu realisieren auf **Datenbankebene**)
#. falls Fläche nicht aufgetrennt wurde und Straßenelementpunkte entstanden sind: Teilelement auf Straßenelement bilden (**noch** zu realisieren auf **Datenbankebene**)
#. falls Fläche aufgetrennt wurde und Straßenelementpunkte entstanden sind: Verknüpfung der jeweiligen Teilelemente und des jeweils betroffenen Straßenelementes (Erfüllung der Bedingung 1..1-Verknüpfung zwischen Straßenelement und Fläche) mit der jeweiligen Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. falls Fläche nicht aufgetrennt wurde und Straßenelementpunkte entstanden sind: Verknüpfung dew Teilelementes und des betroffenen Straßenelementes (Erfüllung der Bedingung 1..1-Verknüpfung zwischen Straßenelement und Fläche) mit der Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. falls Fläche aufgetrennt wurde und keine Straßenelementpunkte entstanden sind: Verknüpfung des jeweils betroffenen Straßenelementes (Erfüllung der Bedingung 1..1-Verknüpfung zwischen Straßenelement und Fläche) mit der jeweiligen Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. falls Fläche nicht aufgetrennt wurde und keine Straßenelementpunkte entstanden sind: Verknüpfung des betroffenen Straßenelementes (Erfüllung der Bedingung 1..1-Verknüpfung zwischen Straßenelement und Fläche) mit der Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. Prüfung der Topologie (**noch** zu realisieren auf **Datenbankebene**)

**Anmerkung:** Im Resultat ist dieser Anwendungsfall identisch mit dem Anwendungsfall :doc:`../flaechen/flaeche-erfassen-trapezmodell`, da in beiden Fällen die Applikationsebene einfach eine Fläche an die Datenbankebene übergibt. Nur die konstruktionsbezogene Herangehensweise auf Applikationsebene ist unterschiedlich. Grundsätzlich gilt: Wurde eine Fläche mittels Zeichnen erfasst, soll sie dennoch mittels Stationierung und Querprofil weiterbearbeitet werden können.

.. _flaeche-erfassen-zeichnen_sachdaten:

Sachdaten
---------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**noch** zu realisieren auf **Applikationsebene**)
* Eingabe aller verpflichtenden und optionalen Attribute (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**schon** realisiert auf **Datenbankebene** über Standardwerte)
* automatisierte Berechnung des Flächeninhaltes in Quadratmetern (**noch** zu realisieren auf **Datenbankebene**)
