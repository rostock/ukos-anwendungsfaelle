.. index:: Flächen, Stationierung, Straßenelemente, Stützpunkte, Teilelemente, Topologie

Fläche löschen
==============

.. image:: /_static/flaeche-loeschen.png

.. _flaeche-loeschen_geometrie:

Geometrie
---------

siehe Präambel, Abschnitt :ref:`Historie <praeambel_historie>`

#. falls Straßenelementpunkte existieren: zugehörige Straßenelementpunkte ebenfalls löschen, falls keine andere, „lebende“ Fläche mehr mit diesen Straßenelementpunkten verknüpft ist (**Datenbankebene**)
#. falls Straßenelementpunkte existieren: Aufhebung der Verknüpfung der Straßenelemente mit der Fläche (**Datenbankebene**)
#. falls Teilelement existiert: zugehöriges Teilelement ebenfalls löschen, falls keine andere, „lebende“ Fläche mehr mit dem Teilelement verknüpft ist (**Datenbankebene**)
#. falls Teilelement existiert: Aufhebung der Verknüpfung des Teilelementes mit der Fläche (**Datenbankebene**)

.. _flaeche-loeschen_sachdaten:

Sachdaten
---------

siehe Präambel, Abschnitt :ref:`Historie <praeambel_historie>`

.. _flaeche-loeschen_verknuepfungen:

Verknüpfungen
-------------

* Löschung aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**Datenbankebene**)
