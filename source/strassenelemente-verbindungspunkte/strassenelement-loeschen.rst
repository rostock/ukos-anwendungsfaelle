.. index:: Stationierung, Straßenelemente, Straßenelementpunkte, Verbindungspunkte

Straßenelement löschen
======================

.. image:: /_static/strassenelement-loeschen.png

.. _strassenelement-loeschen_geometrie:

Geometrie
---------

siehe Präambel, Abschnitt :ref:`Historie <praeambel_historie>`

#. zugehörige Verbindungspunkte ebenfalls löschen, falls kein anderes, „lebendes“ Straßenelement mehr mit den Verbindungspunkten verknüpft ist (**noch** zu realisieren auf **Datenbankebene**)

.. _strassenelement-loeschen_sachdaten:

Sachdaten
---------

siehe Präambel, Abschnitt :ref:`Historie <praeambel_historie>`

.. _strassenelement-loeschen_verknuepfungen:

Verknüpfungen
-------------

* Beibehaltung aller zugehörigen Straßenelementpunkte und Verknüpfungen anderer Objekte mit dem gelöschten Straßenelement sowie keinerlei Änderung oder Löschung verknüpfter anderer Objekte (**noch** zu realisieren auf **Datenbankebene**)
* Aufführung aller Straßenelementpunkte sowie verknüpfter anderer Objekte und Aufforderung zu deren Überprüfung bzw. Anpassung oder Löschung – dabei Implementierung zweier Handlungsmöglichkeiten pro Objekt: a) automatisierte Zuordnung zum nächstgelegenen Straßenelement der Gemeinde, b) manuelle Zuordnung eines beliebigen Straßenelements (**noch** zu realisieren auf **Applikationsebene**)
