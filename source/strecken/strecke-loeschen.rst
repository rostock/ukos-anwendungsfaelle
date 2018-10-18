.. index:: Stationierung, Straßenelemente, Strecken, Stützpunkte, Teilelemente

Strecke löschen
===============

.. image:: /_static/strecke-loeschen.png

.. _strecke-loeschen_geometrie:

Geometrie
---------

siehe Präambel, Abschnitt :ref:`Historie <praeambel_historie>`

#. zugehörigen Start-Straßenelementpunkt ebenfalls löschen, falls keine andere, „lebende“ Strecke mehr mit dem Start-Straßenelementpunkt verknüpft ist (**noch** zu realisieren auf **Datenbankebene**)
#. zugehörigen Ende-Straßenelementpunkt ebenfalls löschen, falls keine andere, „lebende“ Strecke mehr mit dem Ende-Straßenelementpunkt verknüpft ist (**noch** zu realisieren auf **Datenbankebene**)
#. zugehöriges Teilelement auf Start-Straßenelement ebenfalls löschen, falls keine andere, „lebende“ Strecke mehr mit dem Teilelement verknüpft ist (**noch** zu realisieren auf **Datenbankebene**)
#. zugehöriges Teilelement auf Ende-Straßenelement ebenfalls löschen, falls keine andere, „lebende“ Strecke mehr mit dem Teilelement verknüpft ist (**noch** zu realisieren auf **Datenbankebene**)
#. Löschung der Strecke durch Aufhebung der Verknüpfung des Teilelements auf dem Start-Straßenelement, des Teilelements auf dem Ende-Straßenelement und aller dazwischenliegenden Straßenelemente (**noch** zu realisieren auf **Datenbankebene**)

.. _strecke-loeschen_sachdaten:

Sachdaten
---------

siehe Präambel, Abschnitt :ref:`Historie <praeambel_historie>`

.. _strecke-loeschen_verknuepfungen:

Verknüpfungen
-------------

* Löschung aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**noch** zu realisieren auf **Datenbankebene**)
