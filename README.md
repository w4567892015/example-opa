# Open Policy Agent Bundle Example

## Install OPA Cli
```
sudo cp ./opa ./ngrok /bin/
```

## Build Bundle
```
opa build -b bundle -o ./data/bundle.tar.gz
```

## Usage
```
docker-compose up
```

## Test
``` shell
curl -X POST http://localhost:8181/v1/data/authz/allow --data-binary @./data/input.json
```
