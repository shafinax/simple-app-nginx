
# Simple Docker Nginx app with load balancer
This application consist of three docker images and configured load balancing.



## Run Locally

Pull all docker images and run follwoing docker commands

```bash
  docker pull kazishafin/img-app-1
  docker pull kazishafin/img-app-2
  docker pull kazishafin/img-app-3
```


```bash
  docker run -id --name <container-name> -p 80:80 img-app-1
```

```bash
  docker run -id --name <container-name> -p 81:81 img-app-2
```
```bash
  docker run -id --name <container-name> -p 82:82 img-app-3
```

Now! hit localhost on browser and refresh to see the response from load balancer.

## Note

Please use the same port to run container as given.

