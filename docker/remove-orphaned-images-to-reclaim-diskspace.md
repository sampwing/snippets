# Remove orphaned images to reclaim diskspace

If you are building and tagging alot of images eventually you may want to remove unused or orphaned images to reclaim some diskspace.

```
docker rmi $(docker images --filter dangling=true -q)
```
