.. index:: Stationierung, Straßenelemente, Strecken, Stützpunkte

Strecke erfassen
================

.. image:: /_static/strecke-erfassen.png

.. _strecke-erfassen_geometrie:

Geometrie
---------

#. Erfassung des Start-Stützpunktes (**noch** zu realisieren auf **Applikationsebene**)
#. Erfassung des Ende-Stützpunktes (**noch** zu realisieren auf **Applikationsebene**)
#. Auswahl der betroffenen bzw. beteiligten Straßenelement (**noch** zu realisieren auf **Applikationsebene**)
#. Fällung der Lotrechten auf das nächstgelegene betroffene bzw. beteiligte Straßenelement als Vorlaufwert für die Verknüpfung zum Straßenelement (**noch** zu realisieren auf **Applikationsebene**)
#. Fällung der Lotrechten auf das nächstgelegene betroffene bzw. beteiligte Straßenelement zur Ermittlung des Start-Straßenelementpunktes und des Ende-Straßenelementpunktes (**noch** zu realisieren auf **Datenbankebene**)

.. _strecke-erfassen_sachdaten:

Sachdaten
---------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen, zum Beispiel mit einer Straße (über diese dann auch Zuordnung der Organisationseinheit, also der zuständigen Verwaltung) und einer Klassifizierung (**noch** zu realisieren auf **Applikationsebene**)
* Eingabe aller verpflichtenden und optionalen Attribute, zum Beispiel einer Bemerkung (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**schon** realisiert auf **Datenbankebene** über Standardwerte)
* automatisierte Berechnung der Länge in Metern (**noch** zu realisieren auf **Datenbankebene**)
