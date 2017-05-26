# docker-compose Nextcloud

Je nach Leistung des Hostsystems kann es bis zu 2 Minuten dauern bis beim ersten Start alles eingerichtet ist.

'docker logs $(docker ps | grep _nextcloud_1 | awk "{print \$1}")' zeigt:

'SQLSTATE[HY000] [2002] Connection refused' solange bis die DB eingerichtet ist und:

'Nextcloud is not installed' wenn Nextcloud eingerichtet wird und:

'Command line: /usr/sbin/apache2 -D FOREGROUND' sobald Nextcloud läuft.

# docker-compose
