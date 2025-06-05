Netdata Monitoring with Docker

Goal: Get Netdata up and running quickly to monitor your system and apps.

How to run

docker run -d --name=netdata -p 19999:19999 netdata/netdata


Now  

Open http://localhost:19999 in your browser

Watch CPU, memory, disk, and Docker container stats live

Explore alerts and cool charts

Need logs?

docker exec -it netdata tail -f /var/log/netdata/error.log

or simply

docker logs netdata

