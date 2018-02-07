.. index:: Flächen, Stationierung, Straßenelemente, Stützpunkte, Teilelemente, Topologie

Fläche mittels Zeichnen bearbeiten (Geometrie ändern)
=====================================================

.. image:: /_static/flaeche-bearbeiten-zeichnen.png

.. _flaeche-bearbeiten-zeichnen_geometrie:

Geometrie
---------

#. Verschiebung der Stützpunkte einer Fläche als geschlossenes Polygon (**noch** zu realisieren auf **Applikationsebene**)
#. Anpassung der Straßenelementpunkte überall dort, wo die Fläche Straßenelemente schneidet (**noch** zu realisieren auf **Datenbankebene**)
#. falls Fläche über einen oder mehrere Verbindungspunkte hinausgeht: Auftrennung der Fläche an jedem dieser Verbindungspunkte (jeweilige Auftrennungskante beginnt „links“ in jenem Punkt auf der Flächenaußenkante, der die kürzeste Entfernung zum Verbindungspunkt aufweist, geht durch den Verbindungspunkt und endet „rechts“ in jenem Punkt auf der Flächenaußenkante, der die kürzeste Entfernung zum Verbindungspunkt aufweist) (**noch** zu realisieren auf **Datenbankebene**)
#. falls Fläche aufgetrennt wurde und Straßenelementpunkte nach wie vor existieren bzw. entstanden sind: alte Teilelemente löschen und Teilelemente auf Straßenelementen bilden (**noch** zu realisieren auf **Datenbankebene**)
#. falls Fläche nicht aufgetrennt wurde und Straßenelementpunkte nach wie vor existieren bzw. entstanden sind: altes Teilelement löschen und Teilelement auf Straßenelement neu bilden (**noch** zu realisieren auf **Datenbankebene**)
#. falls Fläche aufgetrennt wurde und Straßenelementpunkte nach wie vor existieren bzw. entstanden sind: Verknüpfung der jeweiligen Teilelemente und des jeweils betroffenen Straßenelementes (Erfüllung der Bedingung 1..1-Verknüpfung zwischen Straßenelement und Fläche) mit der jeweiligen Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. falls Fläche nicht aufgetrennt wurde und Straßenelementpunkte nach wie vor existieren bzw. entstanden sind: Neuverknüpfung des Teilelementes und des betroffenen Straßenelementes (Erfüllung der Bedingung 1..1-Verknüpfung zwischen Straßenelement und Fläche) mit der Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. falls Fläche aufgetrennt wurde und keine Straßenelementpunkte nach wie vor existieren bzw. entstanden sind: Verknüpfung des jeweils betroffenen Straßenelementes (Erfüllung der Bedingung 1..1-Verknüpfung zwischen Straßenelement und Fläche) mit der jeweiligen Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. falls Fläche nicht aufgetrennt wurde und keine Straßenelementpunkte nach wie vor existieren bzw. entstanden sind: Neuverknüpfung des betroffenen Straßenelementes (Erfüllung der Bedingung 1..1-Verknüpfung zwischen Straßenelement und Fläche) mit der Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. Prüfung der Topologie (**noch** zu realisieren auf **Datenbankebene**)

**Anmerkung:** Im Resultat ist dieser Anwendungsfall identisch mit dem Anwendungsfall :doc:`../flaechen/flaeche-bearbeiten-trapezmodell`, da in beiden Fällen die Applikationsebene einfach eine Fläche an die Datenbankebene übergibt. Nur die konstruktionsbezogene Herangehensweise auf Applikationsebene ist unterschiedlich. Grundsätzlich gilt: Wurde eine Fläche mittels Zeichnen erfasst, soll sie dennoch mittels Stationierung und Querprofil weiterbearbeitet werden können.

.. _flaeche-bearbeiten-zeichnen_sachdaten:

Sachdaten
---------

* automatisierte Neuberechnung des Flächeninhaltes in Quadratmetern (**noch** zu realisieren auf **Datenbankebene**)

falls Fläche aufgetrennt wurde: siehe Fläche mittels Zeichnen erfassen, Abschnitt :ref:`Sachdaten <flaeche-bearbeiten-zeichnen_sachdaten>`
