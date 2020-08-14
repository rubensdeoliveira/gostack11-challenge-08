<img alt="GoStack" src="https://storage.googleapis.com/golden-wind/bootcamp-gostack/header-desafios.png" />

<h1 align="center">
<br>
Rocketseat - GoStack 11 - Challenge 08
</h1>

<p align="center">
This project was created to solve a challenge requested by Rocketseat.
Gostack is immersive training in technologies, react and react natively.</p>

<p align="center">
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License MIT">
  </a>
</p>

<hr />

## Features

- Features can be accessed by routes below.

- 💹 **Node Js** — A web framework for Node Js

### Routes

- **`POST /customers`**

```json
{
  "name": "José Rubens",
  "email": "jroliveirati@gmail.com",
}
```

- **`POST /products`**

```json
{
	"name": "Fiat argo 1.3",
	"price": 64000.99,
	"quantity": 1
}
```

- **`POST /orders`**

```json
{
  "customer_id": "82e40331-b789-4261-baf0-e726ea4bb139",
	"products": [
		{
			"id": "ebad2d1f-54aa-447e-9ca4-2519eb187e0a",
			"quantity": 1
		},
		{
			"id": "ecd3d802-caa3-4bea-a7c7-0738592f3fb3",
			"quantity": 1
		}
	]
}
```

- **`GET /orders/:id`**

```json
{
  "id": "396316c3-f2a3-4adc-8070-67b132649228",
  "created_at": "2020-08-14T07:14:26.510Z",
  "updated_at": "2020-08-14T07:14:26.510Z",
  "order_products": [
    {
      "id": "ab2149a3-60b1-4c68-8bb4-95825b238bc7",
      "product_id": "ebad2d1f-54aa-447e-9ca4-2519eb187e0a",
      "order_id": "396316c3-f2a3-4adc-8070-67b132649228",
      "price": "64000.49",
      "quantity": 1,
      "created_at": "2020-08-14T07:14:26.510Z",
      "updated_at": "2020-08-14T07:14:26.510Z"
    },
    {
      "id": "91ace1ec-489e-4fac-be5d-6998b391bfbe",
      "product_id": "ecd3d802-caa3-4bea-a7c7-0738592f3fb3",
      "order_id": "396316c3-f2a3-4adc-8070-67b132649228",
      "price": "64000.49",
      "quantity": 1,
      "created_at": "2020-08-14T07:14:26.510Z",
      "updated_at": "2020-08-14T07:14:26.510Z"
    }
  ],
  "customer": {
    "id": "82e40331-b789-4261-baf0-e726ea4bb139",
    "name": "josé",
    "email": "rubensojunior6@gmail.com",
    "created_at": "2020-08-14T06:10:22.697Z",
    "updated_at": "2020-08-14T06:10:22.697Z"
  }
}
```

### Tests

- **`should be able to create a new customer`**

* **`should not be able to create a customer with one e-mail thats already registered`**

- **`should be able to create a new product`**

* **`should not be able to create a duplicated product`**

- **`should be able to create a new order`**

* **`should not be able to create an order with a invalid customer`**

- **`should not be able to create an order with invalid products`**

* **`should not be able to create an order with products with insufficient quantities`**

- **`should be able to subtract an product total quantity when it is ordered`**

* **`should be able to list one specific order`**

## Getting started

- Clone project > enter the project folder
- run `yarn`
- run `docker run --name dbimage -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres`
- Acess postbird or another postgres manager and create db with any name.
- Configure db credentials in src > config > database.js.
- run `yarn typeorm migration:run`
- run `yarn dev:server`

## License

This project is licensed under the MIT License - see the [LICENSE](https://opensource.org/licenses/MIT) page for details.

---

Created with passion by me 👨🏻‍💻
