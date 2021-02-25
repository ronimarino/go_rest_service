# RESTfully Go Service

#### Description:

- Consists of following containers:
  - go web worker
  - phpMyadmin
  - mysql database

- high load processing endpoint
- saving to database in the background
- docker-compose setup
- automatic unit testing
- manual test with GitHub Actions (TODO)

#### USAGE

```docker-compose build```

```docker-compose up```

```ab -p test.json -T application/json -c 100 -n 1000 http://localhost:8080/process```

phpMyAdmin is located on http://localhost:8081  ```root``` / ```root```.

alternative (no docker, uses SQLlite):

```go build```

```./microservice```

```ab -p test.json -T application/json -c 100 -n 10000 http://localhost:8080/process```

