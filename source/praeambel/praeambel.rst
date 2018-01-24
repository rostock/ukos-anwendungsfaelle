.. index:: Bearbeiter, Benutzer, Historie, Metadaten, Präambel, Versionierung

Präambel
========

.. _praeambel_historie:

Historie
--------

Es soll eine Versionierung im Sinne einer Vollhistorie stattfinden: Jede Änderung an einem Objekt, egal ob an Geometrie oder Sachdaten, führt zur Historisierung des Ausgangsobjektes und zur Entstehung eines neuen Objektes; jede Löschung eines Objekts führt zu dessen Historisierung, ohne, dass dabei ein neues Objekt entsteht.

Entsprechende Attribute, mit denen sich eine Versionierung im Sinne einer Vollhistorie realisieren lässt, sind im Datenbankmodell integriert. Umgesetzt werden muss die Versionierung allerdings **noch** auf **Applikationsebene**.

.. _praeambel_bearbeitung:

Metadaten zur Bearbeitung
-------------------------

Es sollen stets Metadaten zur Bearbeitung entstehen, also zum Bearbeiter und zum Zeitpunkt der Bearbeitung.

Entsprechende Attribute, in denen Metadaten zur Bearbeitung abgebildet werden können, sind im Datenbankmodell integriert. Umgesetzt werden muss **noch** die Abbildung der Metadaten auf **Datenbankebene**. Auf  **Applikationsebene** muss dann **noch** realisiert werden, dass die Metadaten zum Bearbeiter anhand des angemeldeten Benutzers an die Datenbankebene übergeben werden.
