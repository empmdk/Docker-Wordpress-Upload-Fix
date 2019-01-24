**Help Us - Help You!**
- Click the Star in the Upper Right Corner to Further promote our Project on GitHub
- Visit the PlexGuide Forum @ http://plexguide.com _(Please Help Our Forum Grow!)_

Part of the http://PlexGuide.com instructions which utilize all docker containers.

## Instructions

- Go to http://ipv4address:9000 (your portainer install)
- [Click] Containers > [Click] Wordpress > [Click] >_Console [Click] Connect

Type the following:

```sh
apt-get update
apt-get install nano
cd /usr/local/etc/php/conf.d/
nano php.ini
```

Copy this into the php.ini document:

```sh
file_uploads = On
memory_limit = 64M
upload_max_filesize = 64M
post_max_size = 64M
max_execution_time = 600
```

Press CTRL + X to Save and then exit and finally type the following

```sh
cp php.ini ..
```

- Click - Disconnect up Top
- Click - Container List on Left or the Server Icon (3rd/4th on Down)
- Look for your Wordpress Container
- Click - Restart
- You will now be able to upload themes that exceed 2MB

Note: to go back to the Wiki, click http://wiki.plexguide.com
