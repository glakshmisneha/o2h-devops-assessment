\# Scenario 1: Docker Container Exits Immediately



Possible Reasons:

1\. Application crash

2\. Wrong CMD or ENTRYPOINT

3\. Missing dependencies

4\. Port conflict



Debug Commands:

docker logs <container\_id>

docker ps -a

docker inspect <container\_id>



\# Scenario 2: Application Works Locally but Not on Server



Checks:

1\. Firewall settings

2\. Open ports

3\. Environment variables

4\. Server logs



Commands:

netstat -tulnp

docker logs <container\_id>

curl http://server-ip:3000

