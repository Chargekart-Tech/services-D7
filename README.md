# ChargeKart

## Web Services Codebase

----

### _Setup_

- Clone the main repository and submodules:
```
git clone -j8 --recurse-submodules --remote-submodules git@github.com:ChargeKart/services.git
```

- Run initialization script:
```
./init.sh
```

- Build and spin up all services
```
docker compose -f docker-compose.dev.yml -p ck-dev up --build -d
```

- To stop the services
```
docker compose -f docker-compose.dev.yml -p ck-dev down
```