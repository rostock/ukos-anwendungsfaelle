.. index:: Flächen, Stationierung, Straßenelemente, Stützpunkte, Teilelemente, Topologie

Fläche mittels Zeichnen bearbeiten (Geometrie ändern)
=====================================================

.. image:: /_static/flaeche-bearbeiten-zeichnen.png

.. _flaeche-bearbeiten-zeichnen_geometrie:

Geometrie
---------

#. Verschiebung der Stützpunkte einer Fläche als geschlossenes Polygon, und zwar nur auf *einem* Straßenelement (also zwischen zwei Verbindungspunkten) (**noch** zu realisieren auf **Applikationsebene**)
#. Anpassung der Straßenelementpunkte überall dort, wo die Fläche Straßenelemente schneidet und dabei *nicht* durch einen Verbindungspunkt geht (**noch** zu realisieren auf **Datenbankebene**)
#. falls Straßenelementpunkte nach wie vor existieren bzw. entstanden sind: altes Teilelement löschen und Teilelement auf Straßenelement neu bilden (**noch** zu realisieren auf **Datenbankebene**)
#. falls Straßenelementpunkte nach wie vor existieren bzw. entstanden sind: Neuverknüpfung des Teilelementes, der Straßenelementpunkte und des betroffenen Straßenelementes mit der Fläche – Erfüllung der Bedingung der Verknüpfung zwischen Straßenelement und Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. falls nach wie vor keine Straßenelementpunkte existieren bzw. entstanden sind: Neuverknüpfung des betroffenen Straßenelementes mit der Fläche – Erfüllung der Bedingung der Verknüpfung zwischen Straßenelement und Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. Prüfung der Topologie (**noch** zu realisieren auf **Datenbankebene**)

**Anmerkung:** Im Resultat ist dieser Anwendungsfall identisch mit dem Anwendungsfall :doc:`../flaechen/flaeche-bearbeiten-trapezmodell`, da in beiden Fällen die Applikationsebene einfach eine Fläche an die Datenbankebene übergibt. Nur die konstruktionsbezogene Herangehensweise auf Applikationsebene ist unterschiedlich. Grundsätzlich gilt: Wurde eine Fläche mittels Zeichnen erfasst, soll sie dennoch mittels Stationierung und Querprofil weiterbearbeitet werden können.

.. _flaeche-bearbeiten-zeichnen_sachdaten:

Sachdaten
---------

* automatisierte Neuberechnung des Flächeninhaltes in Quadratmetern (**noch** zu realisieren auf **Datenbankebene**)

falls Fläche aufgetrennt wurde: siehe Fläche mittels Zeichnen erfassen, Abschnitt :ref:`Sachdaten <flaeche-bearbeiten-zeichnen_sachdaten>`

.. _flaeche-bearbeiten-zeichnen_verknuepfungen:

Verknüpfungen
-------------

* optionale Anpassung aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**noch** zu realisieren auf **Applikationsebene**)
