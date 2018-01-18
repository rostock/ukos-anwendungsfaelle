# *UkoS*-Anwendungsfälle

Anwendungsfälle für *UkoS*, das *Umsetzungsprojekt kommunale Straßendaten Mecklenburg-Vorpommern*

## Hinweis

Die aktuelle Version kann man als Website bei der [*Hanse- und Universitätsstadt Rostock*](https://geo.sv.rostock.de/ukos-anwendungsfaelle) einsehen.

## Voraussetzungen

*   [*Python*](https://www.python.org)
*   [*Virtualenv*](https://virtualenv.pypa.io)

## Installation

1.  neue virtuelle *Python*-Umgebung anlegen, zum Beispiel:

        virtualenv /usr/local/ukos-anwendungsfaelle/virtualenv

1.  Projekt klonen:

        git clone https://github.com/rostock/ukos-anwendungsfaelle /usr/local/ukos-anwendungsfaelle/ukos-anwendungsfaelle

1.  virtuelle *Python*-Umgebung aktivieren:

        source /usr/local/ukos-anwendungsfaelle/virtualenv/bin/activate

1.  benötigte *Python*-Module installieren via [*pip*](https://pip.pypa.io), dem Paketverwaltungsprogramm für *Python*-Pakete:

        pip install -r requirements.txt

## Initialisierung

1.  virtuelle *Python*-Umgebung aktivieren:

        source /usr/local/ukos-anwendungsfaelle/virtualenv/bin/activate

1.  Webseiten bauen:

        make html

## Deployment

Falls die Anwendung mittels [*Apache HTTP Server*](https://httpd.apache.org) deployt werden soll, muss [*mod_wsgi*](http://modwsgi.readthedocs.io) installiert sein, ein Modul, das eine zum Web Server Gateway Interface (WSGI) konforme Schnittstelle für das Hosting *Python*-basierter Web-Anwendungen zur Verfügung stellt. Sofern dies der Fall ist, können folgende Schritte durchgeführt werden:

1.  neue leere Datei `ukos-anwendungsfaelle.wsgi` anlegen:

        touch /usr/local/ukos-anwendungsfaelle/ukos-anwendungsfaelle/ukos-anwendungsfaelle.wsgi
        
1.  Datei `ukos-anwendungsfaelle.wsgi` öffnen und folgenden Inhalt einfügen:
    
        import os
        activate_this = os.path.join('/usr/local/ukos-anwendungsfaelle/virtualenv/bin/activate_this.py')
        with open(activate_this) as file_:
            exec(file_.read(), dict(__file__=activate_this))

        from ukos-anwendungsfaelle import app as application

1.  Konfigurationsdatei des *Apache HTTP Servers* öffnen und in etwa folgenden Inhalt einfügen:
    
        WSGIDaemonProcess    ukos-anwendungsfaelle processes=4 threads=128 python-path=/usr/local/ukos-anwendungsfaelle/ukos-anwendungsfaelle:/usr/local/ukos-anwendungsfaelle/virtualenv/lib/python2.7/site-packages
        WSGIProcessGroup     ukos-anwendungsfaelle
        WSGIScriptAlias      /ukos-anwendungsfaelle /usr/local/ukos-anwendungsfaelle/ukos-anwendungsfaelle/ukos-anwendungsfaelle.wsgi process-group=ukos-anwendungsfaelle
        
        <Directory /usr/local/ukos-anwendungsfaelle/ukos-anwendungsfaelle>
            Order deny,allow
            Require all granted
        </Directory>
