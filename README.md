# MyRasp as a WebServer

1. Follow the Securing your Raspberry blog:
https://www.raspberrypi.org/documentation/configuration/security.md

1. Configure ufw to allow the ports: ` ufw allow 50022 ` ` ufw allow 5000 `

1. Configure no-ip and DUC at:
https://www.noip.com/support/knowledgebase/install-ip-duc-onto-raspberry-pi/

1. Force update: ` sudo /usr/local/bin/noip2 `

1. Check if noip is running: ` noip2 -S `

1. Setup the virtual ports on the router.
50022 ssh 5000 flask app.

1. Get the temperature of the rapsberry: ` vcgencmd measure_temp `

1. To run as a regular user: ` sudo chmod u+s /opt/vc/bin/vcgencmd `



### TO DO
- run the app inside a docker container
- upload the code to github
- on changes, download and run on docker container
- Long run: create a notification on syntax issues.
