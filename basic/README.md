# splunk

### Run splunk in a docker container

1. Start up Splunk:
```
docker run --rm -d -p 8000:8000 -e "SPLUNK_START_ARGS=--accept-license" -e "SPLUNK_PASSWORD=qwerty123" --name splunk splunk/splunk:latest
```
Splunk will be availbale on the URL:
```
http://localhost:8000/
User: admin
Pass: qwerty123
```
```
docker stop splunk
```
### List all possible indexes:
```
| eventcount summarize=false index=* index=_* | dedup index | fields index
```
`index=_*` relates to interal indexes

### Run splunk uing docker-compose
1. Start up Splunk
```
docker-compose up -d
```
2. Check a running container and exposed port
```
docker ps

CONTAINER ID   IMAGE                  COMMAND                  CREATED       STATUS                            PORTS                                                                                                NAMES
b9ed545cba8e   splunk/splunk:latest   "/sbin/entrypoint.sh…"   2 weeks ago   Up 5 seconds (health: starting)   8065/tcp, 8088/tcp, 8191/tcp, 9887/tcp, 9997/tcp, 0.0.0.0:55328->8000/tcp, 0.0.0.0:55329->8089/tcp   so1
```
The port `55328` is an external port which is mapped to `8080`.
It can be use to access Splunk:
```
http://localhost:55328
```
Use the same credentials to log in:
User: admin
Pass: qwerty123

3. Stop Splunk
```
docker-compose stop
```
### Free license
When a trial license expires you have to swith to Free one. 

To switch licenses:

* Log in to Splunk Web as a user in the admin role
* Select **Settings > Licensing**
* Click **Change License Group**
* Select **Free license**
* Click **Save**
* You are prompted to restart

More details: see [How do I switch to the Splunk Free license?](https://docs.splunk.com/Documentation/Splunk/9.0.1/Admin/MoreaboutSplunkFree)


### References
* [docker-splunk](https://splunk.github.io/docker-splunk/STORAGE_OPTIONS.html)
