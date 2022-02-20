# payroll-rest-api
Payroll Rest API demo using Java spring


### Running the API Rest
```shell
./mvnw clean spring-boot:run
```

### Accession the API Rest
```shell
curl -v localhost:8080/employees
curl -v localhost:8080/employees/99
curl -X POST localhost:8080/employees -H 'Content-type:application/json' -d '{"name": "Samwise Gamgee", "role": "gardener"}'
curl -v localhost:8080/employees/3
curl -X PUT localhost:8080/employees/3 -H 'Content-type:application/json' -d '{"name": "Samwise Gamgee", "role": "ring bearer"}'
curl -v localhost:8080/employees/3
curl -X DELETE localhost:8080/employees/3
curl -v localhost:8080/employees/3

curl -v localhost:8080/employees/1 | json_pp
curl -v localhost:8080/employees | json_pp


```
