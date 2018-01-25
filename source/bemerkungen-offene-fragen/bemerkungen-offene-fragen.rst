Bemerkungen und offene Fragen
=============================

.. _bemerkungen-offene-fragen_konvertierung-flaechen-in-linien:

Sollen Flächen im Landesmodell aufgenommen oder in ein linienhaftes Format konvertiert werden?
----------------------------------------------------------------------------------------------

Dies hätte Auswirkungen auf die Anwendungsfälle :doc:`../flaechen/flaeche-erfassen`, :doc:`../flaechen/flaeche-bearbeiten` und :doc:`../flaechen/flaeche-erzeugen`!

.. _bemerkungen-offene-fragen_erzeugte-flaeche-bearbeiten:

Soll es die Möglichkeit geben, aus Stationierung und Querprofil erzeugte Flächen über Änderung von Stationierung und Querprofil zu bearbeiten?
----------------------------------------------------------------------------------------------------------------------------------------------

Falls ja, müsste es dazu ein neuer Anwendungsfall *Fläche bearbeiten, die aus Stationierung und Querprofil erzeugt wurde* angelegt werden.

.. _bemerkungen-offene-fragen_verhaeltnis-flaeche-strassenelement:

Wie soll das Verhältnis zwischen Flächen und Straßenelementen genau gestaltet sein?
-----------------------------------------------------------------------------------

Möglichkeit 1
^^^^^^^^^^^^^

Eine Fläche soll mit 1..n Straßenelementen verknüpft werden können. Dann wären die Graphiken in den Anwendungsfällen :doc:`../flaechen/flaeche-erfassen`, :doc:`../flaechen/flaeche-bearbeiten` und :doc:`../flaechen/flaeche-loeschen` korrekt, es müssten aber eventuell die jeweiligen Texte angepasst werden.

Möglichkeit 2
^^^^^^^^^^^^^

Eine Fläche soll mit 1 Straßenelement verknüpft werden können. Dann wären die Texte in den Anwendungsfällen :doc:`../flaechen/flaeche-erfassen`, :doc:`../flaechen/flaeche-bearbeiten` und :doc:`../flaechen/flaeche-loeschen` korrekt, es müssten aber auf jeden Fall die jeweiligen Graphiken angepasst werden: Die linke Begrenzungslinie der Fläche M und die rechte von N müssten dann jeweils zwingend durch einen Verbindungspunkt laufen.

Möglichkeit 3
^^^^^^^^^^^^^

Flächen soll nicht mit Straßenelementen verknüpft werden können, sondern mit Straßen.
