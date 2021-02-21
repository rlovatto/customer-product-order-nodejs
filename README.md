# Node.js - Customers, Products, Orders project
Exercise on Node.js for the Bootcamp GoStack - Rocketseat

It is a rest api that is possible to add customers, products and orders.

To install all dependencies:

```
yarn
```

To run the project:

```
yarn dev:server
```

### Endpoints:

POST   - /customers <br>
```json
{
	"name": "Robinson",
	"email": "robinson@example.com"
}
```


POST   - /products <br>
```json
{
	"name": "Guitar",
	"price": 200.3,
	"quantity": 30
}
```

POST   - /orders <br>
```json
{
	"customer_id": "bcf09397-24f6-411d-bfe4-705e5c7c9fa0",
	"products":[
		{
			"id": "a51924e7-fc39-4c61-9107-d0235144b371",
			"quantity": 2
		}
	]
}
```

GET    - /orders/:id <br>
```json
{
  "id": "b2d83c4c-85bc-4982-b72b-fea3c7bb91f0",
  "created_at": "2021-02-20T16:48:51.693Z",
  "updated_at": "2021-02-20T16:48:51.693Z",
  "order_products": [
    {
      "id": "2c8b8aa0-3420-45a0-a077-51618729c6a8",
      "product_id": "a51924e7-fc39-4c61-9107-d0235144b371",
      "order_id": "b2d83c4c-85bc-4982-b72b-fea3c7bb91f0",
      "price": "200.30",
      "quantity": 2,
      "created_at": "2021-02-20T16:48:51.693Z",
      "updated_at": "2021-02-20T16:48:51.693Z"
    }
  ],
  "customer": {
    "id": "bcf09397-24f6-411d-bfe4-705e5c7c9fa0",
    "name": "Robinson",
    "email": "robinson@example.com",
    "created_at": "2021-02-20T14:35:18.632Z",
    "updated_at": "2021-02-20T14:35:18.632Z"
  }
}
```

There is no front-end for this project.
