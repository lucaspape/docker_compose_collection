After ```docker-compose up -d``` make sure to ```docker-compose exec nextcloud chown www-data /srv/nextcloud/data/``` (otherwise no permission to write data dir)

To fix some nextcloud proxy issues: add ```'overwriteprotocol' => 'https'```, to ```root/html/config/config.php``` 
