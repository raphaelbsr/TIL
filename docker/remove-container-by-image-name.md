# Today I Learn

### Remove docker containers based on image name

```bash
docker ps -a | awk '{ print $1,$2 }' | grep mariadb | awk '{print $1 }' | xargs -I {} docker rm {}
```

### Links

[reference](https://gist.github.com/alrayyes/d35c288f3005181cefb38d2df4e955e8)
