### Quick Start of the Hedgehog Cloud
```
cd /srv
git clone https://github.com/eigener-server/docker-compose.git eigener-server.ch
cd eigener-server.ch
sed -i -e "s#192.168.1.0/24#YOUR-REMOTE-ADMIN-ACCESS-IP/SUBNET#g" docker-compose.yml
sed -i -e "s#192.168.1.97#YOUR-SERVER-IP_or_DOMAIN#g" docker-compose.yml
./up
```

### License of the Hedgehog Cloud

You may duplicate and redistribute the material in any format or medium as well as refix, alter, and build
upon the material for any purpose, even commercially.


The following conditions must be observed:
Attribution — You must provide a link to our website (www.eigener-server.ch/en/igel-cloud) on your website
Website. We prefer the footer.

Removing the link — We understand that there are situations where you do not want to use a link reference.
If that is your case, then you can transfer us a usage fee of 10 CHF by Paypal. This allows you to use the
hedgehog cloud free of charge on a domain.

You can send your payments via Paypal to the following address: igel-cloud@nextora.ch
Please note the URL of the website, where the hedgehog cloud is used, as a remark with the Paypal Payment.
Keep your Paypal receipt as proof of payment.

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/">
<img alt="Creative Commons Lizenzvertrag" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/80x15.png" />
</a>

Hedgehog Cloud by <a rel="license" href="https://www.eigener-server.ch/en/igel-cloud">www.eigener-server.ch</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Namensnennung 4.0 International Lizenz</a>.



# docker-compose Nextcloud

Je nach Leistung des Hostsystems kann es bis zu 2 Minuten dauern bis beim ersten Start alles eingerichtet ist.

'docker logs $(docker ps | grep _nextcloud_1 | awk "{print \$1}")' zeigt:

'SQLSTATE[HY000] [2002] Connection refused' solange bis die DB eingerichtet ist und:

'Nextcloud is not installed' wenn Nextcloud eingerichtet wird und:

'Command line: /usr/sbin/apache2 -D FOREGROUND' sobald Nextcloud läuft.

# docker-compose
