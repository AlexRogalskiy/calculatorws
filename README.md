# CALCULATOR WS
---
**CalculatorWS** is a REST web service implemented in Java using the framework Spring Boot. 
It uses RabbitMQ for the communications between two modules that exists in the WS, **Rest** and **Calculator**. The WS supports the following math operations:  
- Addition
- Subtraction
- Multiplication
- Division

## API's
---

### Addition (sum)
```sh
curl \
--header "Content-type: application/json" \
--request GET \
"http://localhost:8080/sum?a={num1}&b={num2}"
```
### Example
```sh
curl \
--request GET \
"http://localhost:8080/sum?a=10&b=5"
...
HTTP/1.1 200 OK Content-Type: application/json
{"result":15}
```
---

### Subtraction (sub)
```sh
curl \
--header "Content-type: application/json" \
--request GET \
"http://localhost:8080/sub?a={num1}&b={num2}"
```
#### Example
```sh
curl \
--request GET \
"http://localhost:8080/sub?a=10&b=5"
...
HTTP/1.1 200 OK Content-Type: application/json
{"result":5}
```
---

### Multiplication (mul)
```sh
curl \
--header "Content-type: application/json" \
--request GET \
"http://localhost:8080/mul?a={num1}&b={num2}"
```
#### Example
```sh
curl \
--request GET \
"http://localhost:8080/mul?a=10&b=5"
...
HTTP/1.1 200 OK Content-Type: application/json
{"result":50}
```
---

### Division (div)
```sh
curl \
--header "Content-type: application/json" \
--request GET \
"http://localhost:8080/divb?a={num1}&b={num2}"
```
#### Example
```sh
curl \
--request GET \
"http://localhost:8080/div?a=10&b=5"
...
HTTP/1.1 200 OK Content-Type: application/json
{"result":2}
```