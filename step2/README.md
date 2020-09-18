## Step 2

In this step we will connect to the machine running Grafana.

This is necessary because plugins have to be installed in a specific folder.


Start the app:
```
docker-compose up -d
```

Once up, run 
```
docker ps --format "table {{.Names}}" --filter "name=grafana"
```

Using the image name from the command above, access the image using:

```
docker exec -it step2_grafana_1 sh
```

While there, check the folder `/etc/grafana` and the file `grafana.ini` inside of it.


You can exit the image with `exit`.

## What did we do so far?

We are able to access Grafana under the hood.