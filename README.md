```
curl --silent -X GET "http://localhost:4000/ping" | jq
curl --silent -X GET "http://localhost:4000/products" | jq
curl --silent -X GET "http://localhost:4000/products/laptop" | jq
curl --silent -X POST -H "Content-Type: application/json" -d '{"name":"mouse", "price":40, "quantity":40}' "http://localhost:4000/products" | jq
curl --silent -X PUT -H "Content-Type: application/json" -d '{"name":"mouse", "price":400, "quantity":400}' "http://localhost:4000/products/mouse" | jq
curl --silent -X DELETE "http://localhost:4000/products/mouse" | jq
```
