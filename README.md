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
List all possible indexes:
```
| eventcount summarize=false index=* index=_* | dedup index | fields index
```
### Run splunk uing docker-compose
1. Start up Splunk
```
docker-compose up -d
```
2. Stop Splunk
```
docker-compose stop -d
```


### References
* [docker-splunk](https://splunk.github.io/docker-splunk/STORAGE_OPTIONS.html)
