# vlib nagios Konfiguration
2011-2013 Sven-S. Porst, SUB Göttingen <porst@sub.uni-goettingen.de>

Konfigurationsdateien des nagios Dienstes auf dem VLib Testserver. Hauptsächlich zum Testen der Dienste für die virtuellen Fachbibliotheken.

## Konfigurationsdateien im Ordner sub
* commands.cfg: Eigene Befehle, die in den weiteren Konfigurationsdateien genutzt werden
* contacts.cfg: Kontaktdaten für E-Mails, die in den weiteren Konfigurationsdateien genutzt werden
* groups.cfg: Konfiguration zur Gruppierung einzelner Abfragen nach Servicezugehörigkeit
* vlib.cfg: Test der virtuellen Fachbibliotheken, des fabian Wiki und des VLib Testservers
* pazpar2.cfg: Test des pazpar2 Servers
* bibliographic-servers.cfg: Test von SRU und Z39.50 Servern, die für die Metasuchen genutzt werden
* solr-harvest.cfg: Test der Solr Indexe für das Harvesting
* sru.cfg: Test des SRU Servers
* opac.cfg: SUB Göttingen OPAC Tests nach Verfügbarkeit, incl spezielle Indexe und Ausgabeformate
* zvdd.cfg: Test des ZVDD Webservers
* cerl.cfg: Test des CERL Webservers und CERL Thesaurus

## Eigene Testskripte in sub/yaz
Das Skript »check_yaz« stellt einen nagios Testbefehl für den yaz-client zur Verfügung. Es führt ein yaz-client Skript aus und gibt eine nagios konforme Ausgabe zurück.

Die weiteren Dateien sind kleine yaz-client Skripte, die zur Überprüfung der einzelen Server genutzt werden.