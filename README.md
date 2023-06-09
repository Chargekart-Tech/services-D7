# ChargeKart D7

## Web Services Codebase

----

### _Setup_

- Clone the main repository and submodules:
```
git clone -j8 --recurse-submodules --remote-submodules git@github.com:Chargekart-Tech/services-D7.git
```

- Pull latest changes for the submodules
```
git pull --recurse-submodules
```

- Run initialization script:
```
./init.sh
```

If you get an error, please run the following command and try again:
```
chmod +x init.sh
```

- Build and spin up all services
```
docker compose -f docker-compose.dev.yml -p ck-d7-dev up --build -d
```

- To stop the services (Without removing the MongoDB data)
```
docker compose -f docker-compose.dev.yml -p ck-d7-dev down
```
