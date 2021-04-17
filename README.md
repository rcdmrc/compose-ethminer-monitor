# Usage

Clone this repo and initialize:
```shell
git clone <this repo>
git submodule update --init --recursive
```

Now start the containers:
```shell
docker-compose up -d fluentd prometheus grafana
sleep 5 # need to wait a bit until fluentd is ready.
docker-compose up -d ethminer
```

Point your web browser to the grafana service at http://localhost:9000.