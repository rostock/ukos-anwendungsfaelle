.. index:: Begleitobjekte, Einfügebasispunkte, Punktobjekte, Stationierung, Straßenelemente, Stützpunkte

Punktobjekt erfassen
====================

.. image:: /_static/punktobjekt-erfassen.png

.. _punktobjekt-erfassen_geometrie:

Geometrie
---------

.. _punktobjekt-erfassen_moeglichkeit-1:

Möglichkeit 1
^^^^^^^^^^^^^

#. Erfassung des Einfügebasispunktes eines Punktobjektes (Begleitobjektes) (**noch** zu realisieren auf **Applikationsebene**)
#. Fällung der Lotrechten auf das nächstgelegene Straßenelement als Vorlaufwert für die Verknüpfung zum Straßenelement (**noch** zu realisieren auf **Applikationsebene**)
#. Fällung der Lotrechten auf das nächstgelegene Straßenelement, Erstellung eines Straßenelementpunktes und Berechnung des Abszissenwertes, des Ordinatenwertes sowie der Ordinatenrichtung (**noch** zu realisieren auf **Datenbankebene**)

.. _punktobjekt-erfassen_moeglichkeit-2:

Möglichkeit 2
^^^^^^^^^^^^^

#. Ermittlung der Einfügekoordinate des Punktobjektes (Begleitobjektes) durch Eingabe der Abszissen- und Ordinatenwerte sowie der Ordinatenrichtung (**noch** zu realisieren auf **Applikationsebene**)
#. Erzeugung der Einfügekoordinate (**noch** zu realisieren auf **Datenbankebene**)

.. _punktobjekt-erfassen_sachdaten:

Sachdaten
---------

* Eingabe aller gemäß Datenbankmodell verpflichtenden Verknüpfungen (**noch** zu realisieren auf **Applikationsebene**)
* Eingabe aller verpflichtenden und optionalen Attribute (**noch** zu realisieren auf **Applikationsebene**)
* automatisierte Erstellung aller weiteren verpflichtenden Attribute, zum Beispiel der UUID (**schon** realisiert auf **Datenbankebene** über Standardwerte)
