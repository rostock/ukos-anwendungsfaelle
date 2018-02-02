.. index:: Flächen, Querprofil, Stationierung, Straßenelemente, Stützpunkte, Teilelemente, Topologie

Fläche mittels Stationierung und Querprofil bearbeiten (Geometrie im „Trapezmodell“ ändern)
===========================================================================================

.. _flaeche-bearbeiten-trapezmodell_geometrie:

Geometrie
---------

#. Verschiebung von Straßenelementpunkten und/oder Änderung von Querprofilen (**noch** zu realisieren auf **Applikationsebene**):
    * optionale Verschiebung des Start-Straßenelementpunktes und damit zugleich Neufestlegung des Start-Straßenelements
    * optionale Verschiebung des Ende-Straßenelementpunktes und damit zugleich Neufestlegung des Ende-Straßenelements
    * optionale Verschiebung, Löschung und/oder Erfassung der dazwischenliegenden Straßenelementpunkte für die Querprofile
    * optionale Neuingabe der L- und/oder R-Ordinaten der Querprofile an jedem dazwischenliegenden Straßenelementpunkt für die Querprofile
#. Anpassung der Fläche als geschlossenes Polygon (**noch** zu realisieren auf **Applikationsebene**)
#. Teilelement auf Start-Straßenelement (von Start-Straßenelementpunkt bis nächsten Verbindungspunkt in Richtung Ende-Straßenelement) neu bilden (**noch** zu realisieren auf **Datenbankebene**)
#. Teilelement auf Ende-Straßenelement (von nächstem Verbindungspunkt aus Richtung Start-Straßenelement bis Ende-Straßenelementpunkt) neu bilden (**noch** zu realisieren auf **Datenbankebene**)
#. alte Teilelemente löschen
#. Neuverknüpfung der Teilelemente und der dazwischenliegenden Straßenelemente mit der Fläche (**noch** zu realisieren auf **Datenbankebene**)
#. Prüfung der Topologie (**noch** zu realisieren auf **Datenbankebene**)

**Anmerkung:** Im Resultat ist dieser Anwendungsfall identisch mit dem Anwendungsfall :doc:`../flaechen/flaeche-erfassen-zeichnen`, da in beiden Fällen die Applikationsebene einfach eine Fläche an die Datenbankebene übergibt. Nur die konstruktionsbezogene Herangehensweise auf Applikationsebene ist unterschiedlich. Grundsätzlich gilt: Wurde eine Fläche mittels Stationierung und Querprofil erfasst, soll sie dennoch mittels Zeichnen weiterbearbeitet werden können.

.. _flaeche-bearbeiten-trapezmodell_sachdaten:

Sachdaten
---------

* automatisierte Neuberechnung des Flächeninhaltes in Quadratmetern (**noch** zu realisieren auf **Datenbankebene**)
