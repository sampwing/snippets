# Remove orphaned volumes to reclaim diskspace

```
docker volume rm $(docker volume ls --filter dangling=true -q)
```
