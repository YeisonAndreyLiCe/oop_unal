# AmazonUnal

Diagrama UML: https://drive.google.com/file/d/1v7ovKShlE6WO656TTvB5s7eh_KFZIz5b/view?usp=drive_link

## Descripción

Este proyecto permite a los usuarios buscar productos y comprar productos. Igualmente se permite la
adición de productos al carrito de compras y la eliminación de productos del carrito de compras.
Tendremos un manejo de inventario que verificará disponibilidad, precios y cantidades de los productos.
Los usuarios que quieran interactual con la aplicación deberán registrarse y loguearse.
Adicionalmente se podrá agregar comentarios a los productos y calificarlos.

Por Facilidad Tendremos un usuario ya registrado que podrá llevar a cabo todas las acciones de la aplicación.

No vamos a usar bases de datos en su lugar usaremos archivos json para almacenar la información en la carpeta data.

<!-- json user example -->

Ejemplo de un usuario:

```json
{
  "id": "jonhdoe@gmail.com",
  "name": "Jonh Doe",
  "password": "a_very_secure_password",
  "address": {
    "street": "Calle 123",
    "city": "Medellín",
    "country": "Colombia"
  },
  "paymentMethod": {
    "card": "1234-1234-1234-1234",
    "expiration": "12/23",
    "cvv": "123"
  },
  "paymentsHistory": [
    {
      "id": "123",
      "date": "2021-10-10",
      "products": [
        {
          "id": "123",
          "name": "Product 1",
          "price": 1000,
          "quantity": 2
        },
        {
          "id": "124",
          "name": "Product 2",
          "price": 2000,
          "quantity": 1
        }
      ],
      "total": 3000
    }
  ]
}
```

<!-- json product example -->

Ejemplo de un producto:
```json
{
  "id": "123",
  "name": "Product 1",
  "price": 1000,
  "quantity": 10,
  "comments": [
    {
      "user": "jondoe@gmail.com",
        "comment": "This is a great product",
        "rating": 5
    }
    ]
}
```
