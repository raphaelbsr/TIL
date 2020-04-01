# Today I Learn

### Run a bitnami/redis image

To run a bitnami/redis container with persistent storage maped to the host, we need to change folder permissions to avoid restrictions access

```bash
sudo chown -R 1001:1001 redis/
```

### Links

[Stackoverflow](https://github.com/bitnami/bitnami-docker-redis/issues/89#issuecomment-345608149)

[Bitnami Redis Doc](https://github.com/bitnami/bitnami-docker-redis)
