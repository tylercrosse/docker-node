# Node-Docker
Simple express app running on docker

### Build
To build and tag the image
```
$ docker build -t <your username>/node-web-app .
```

### Run
To run the image and expose the port bound to express as 49160. This command will also name the image `node-web-app`
```
$ docker run -p 49160:8080 --name node-web-app -d <your username>/node-web-app 
```

After running the above command the image can be stopped and started simple commands using the image name.
```
$ docker stop node-web-app
```
```
$ docker start node-web-app
```

### Test
You can test the app once the image is running by visiting `localhost:49160`

or with curl:
```
$ curl -i localhost:49160
```