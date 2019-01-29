```
docker run -it \
-e MONGODB_ADMIN_USER=admin \
-e MONGODB_ADMIN_PASS=adminpass \
-e MONGODB_APPLICATION_DATABASE=mytestdatabase \
-e MONGODB_APPLICATION_USER=testuser \
-e MONGODB_APPLICATION_PASS=testpass \
-p 27017:27017 volyihin/mongo:3.4
```

Bind the /data/db folder to a local folder (add the -v parameter to docker run):  docker run -it … -v /path/to/local/folder:/data/db volyihin/mongo:3.4