.. index:: Flächen, Querprofil, Stationierung, Straßenelemente, Stützpunkte, Teilelemente, Topologie

Fläche mittels Stationierung und Querprofil bearbeiten (Geometrie im „Trapezmodell“ ändern)
===========================================================================================

.. image:: /_static/flaeche-bearbeiten-trapezmodell.png

.. _flaeche-bearbeiten-trapezmodell_geometrie:

Geometrie
---------

#. Verschiebung von Straßenelementpunkten und/oder Änderung von Querprofilen, und zwar nur auf *einem* Straßenelement (also zwischen zwei Verbindungspunkten) (**Applikationsebene**):
    * optionale Verschiebung des Start-Straßenelementpunktes oder Neuauswahl des Start-Verbindungspunktes
    * optionale Verschiebung des Ende-Straßenelementpunktes oder Neuauswahl des Ende-Verbindungspunktes
    * optionale Verschiebung, Löschung und/oder Erfassung der dazwischenliegenden Straßenelementpunkte
    * optionale Neuingabe aller L- und/oder R-Ordinaten der Querprofile
#. Anpassung der Querschnittsflächen als einzelne, geschlossene Polygone (**Applikationsebene**)
#. falls Straßenelementpunkte entstanden sind: Teilelemente auf Straßenelement bilden (**Datenbankebene**)
#. falls Straßenelementpunkte entstanden sind: Verknüpfung der Teilelemente, der Straßenelementpunkte und des betroffenen Straßenelementes mit jeweils passender Querschnittsfläche – Erfüllung der Bedingung der Verknüpfung zwischen Straßenelement und Fläche (**Datenbankebene**)
#. falls keine Straßenelementpunkte entstanden sind: Verknüpfung des betroffenen Straßenelementes mit der Querschnittsfläche – Erfüllung der Bedingung der Verknüpfung zwischen Straßenelement und Fläche (**Datenbankebene**)
#. Prüfung der Topologie (**Datenbankebene**)
#. Anpassung der verknüpften, übergeordneten Verkehrsfläche (**Datenbankebene**)

**Anmerkung:** Im Resultat ist dieser Anwendungsfall identisch mit dem Anwendungsfall :doc:`../flaechen/flaeche-erfassen-zeichnen`, da in beiden Fällen die Applikationsebene einfach Flächen an die Datenbankebene übergibt. Nur die konstruktionsbezogene Herangehensweise auf Applikationsebene ist unterschiedlich. Grundsätzlich gilt: Wurde eine Fläche mittels Stationierung und Querprofil erfasst, soll sie dennoch mittels Zeichnen weiterbearbeitet werden können.

.. _flaeche-bearbeiten-trapezmodell_sachdaten:

Sachdaten
---------

* automatisierte Neuberechnung des Flächeninhaltes in Quadratmetern (**Datenbankebene**)

.. _flaeche-bearbeiten-trapezmodell_verknuepfungen:

Verknüpfungen
-------------

* optionale Anpassung aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**Applikationsebene**)
