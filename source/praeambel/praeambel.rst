.. index:: Bearbeiter, Historie, Metadaten, Präambel, Versionierung

Präambel
========

.. _praeambel_historie:

Historie
--------

Es soll eine Versionierung im Sinne einer Vollhistorie stattfinden: Jede Änderung an einem Objekt, egal ob an Geometrie oder Sachdaten, führt zur Historisierung des Ausgangsobjektes und zur Entstehung eines neuen Objektes; jede Löschung eines Objekts führt zu dessen Historisierung, ohne, dass dabei ein neues Objekt entsteht.

Entsprechende Attribute, mit denen sich eine Versionierung im Sinne einer Vollhistorie realisieren lässt, sind im Datenbankmodell integriert. Umgesetzt werden muss die Versionierung allerdings **noch** auf **Applikationsebene**.

Historische Objekte sollen zwar standardmäßig nicht (mehr) zur Darstellung gebracht werden, es soll aber die Möglichkeit bestehen, historische Objekte zu reaktivieren – Beispiel: Ein Papierkorb, der einige Zeit zur Reparatur abgebaut war, soll wieder installiert werden. Auch dies ist **noch** zu realisieren auf **Applikationsebene**.

.. _praeambel_ident:

„Ident“ und „historische Ident“
-------------------------------

Nicht nur neue Straßenelemente und Verbindungspunkte, sondern auch alle doppischen Objekte erhalten stets eine sogenannte „Ident“, das heißt einen eindeutigen Code bestehend aus 6 Zeichen der Menge [0-9a-zA-Z]. Es ist sichergestellt, dass „Idents“ nicht mehrfach vorkommen, auch über Objektgrenzen hinweg – das heißt, dass zum Beispiel ein Straßenelement niemals denselben „Ident“ aufweisen wird wie etwa ein Verbindungspunkt oder ein Papierkorb. Dies ist **schon** realisiert auf **Datenbankebene**.

Nicht nur Straßenelemente und Verbindungspunkte, sondern auch alle doppischen sowie weitere Objekte können (müssen aber nicht) eine „historische Ident“ zugewiesen bekommen. Dies ist vor allem dann sinnvoll, wenn diese Objekte aus externen Datenbeständen importiert wurden. Dies ist **schon** realisiert auf **Datenbankebene**.

.. _praeambel_bearbeitung:

Metadaten zur Bearbeitung
-------------------------

Es sollen stets Metadaten zur Bearbeitung entstehen, also zum Bearbeiter und zum Zeitpunkt der Bearbeitung.

Entsprechende Attribute, in denen Metadaten zur Bearbeitung abgebildet werden können, sind im Datenbankmodell integriert. Umgesetzt werden muss **noch** die Abbildung der Metadaten auf **Datenbankebene**. Auf  **Applikationsebene** muss dann **noch** realisiert werden, dass die Metadaten zum Bearbeiter anhand des angemeldeten Benutzers an die Datenbankebene übergeben werden.
