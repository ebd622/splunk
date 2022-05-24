# splunk

```
docker run --rm -d -p 8000:8000 -e "SPLUNK_START_ARGS=--accept-license" -e "SPLUNK_PASSWORD=qwerty123" --name splunk splunk/splunk:latest
```
```
docker stop splunk
```
