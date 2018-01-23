# *UkoS*-Anwendungsfälle

Anwendungsfälle für *UkoS*, das *Umsetzungsprojekt kommunale Straßendaten Mecklenburg-Vorpommern*; gehostet bei der Hanse- und Universitätsstadt Rostock unter https://geo.sv.rostock.de/ukos-anwendungsfaelle

## Voraussetzungen

*   [*Python*](https://www.python.org)
*   [*Virtualenv*](https://virtualenv.pypa.io)

## Installation

1.  neue virtuelle *Python*-Umgebung anlegen, zum Beispiel:

        virtualenv /srv/www/htdocs/ukos-anwendungsfaelle/virtualenv

1.  Projekt klonen:

        git clone https://github.com/rostock/ukos-anwendungsfaelle /srv/www/htdocs/ukos-anwendungsfaelle/ukos-anwendungsfaelle

1.  virtuelle *Python*-Umgebung aktivieren:

        source /srv/www/htdocs/ukos-anwendungsfaelle/virtualenv/bin/activate

1.  benötigte *Python*-Module installieren via [*pip*](https://pip.pypa.io), dem Paketverwaltungsprogramm für *Python*-Pakete:

        pip install -r requirements.txt

## Initialisierung

1.  virtuelle *Python*-Umgebung aktivieren:

        source /srv/www/htdocs/ukos-anwendungsfaelle/virtualenv/bin/activate

1.  Webseiten bauen:

        make html

## Deployment (am Beispiel des [*Apache HTTP Servers*](https://httpd.apache.org))

1.  Konfigurationsdatei des *Apache HTTP Servers* öffnen und in etwa folgenden Inhalt einfügen:
    
        Alias /ukos-anwendungsfaelle /srv/www/htdocs/ukos-anwendungsfaelle/ukos-anwendungsfaelle/build/html

        <Directory /srv/www/htdocs/ukos-anwendungsfaelle/ukos-anwendungsfaelle/build/html>
            Order deny,allow
            Require all granted
        </Directory>
