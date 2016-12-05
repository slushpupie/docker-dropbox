Run dropbox inside a docker container.

Docker run example:

```
docker run -d --name dropbox -v /path/to/local/config:/root/.dropbox -v /path/to/DB/files/folder:/root/Dropbox -v /etc/localtime:/etc/localtime:ro slushpupie/dropbox:latest
```

To check up on current status:

```
docker exec dropbox dropbox.py status
```
