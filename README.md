# Instructions to run application

git clone https://github.com/ssuryaw5/semantic-web-crime-ontology

```bash
cd semantic-web-crime-ontology
```

download data.zip file uploaded on canvas. Upload the data folder inside semantic-web-crime-ontology

Make sure you have docker installed on the device (https://docs.docker.com/engine/install/)
Run the docker deamon

Run the following command to start the application

### To start the application

```bash
docker-compose -f docker-compose.services.yaml up
```

### Click below link to test the application

[web-semantic-crime-analysis-app](http://localhost:8080)

### To stop the application

```bash
docker-compose -f docker-compose.services.yaml down
```
