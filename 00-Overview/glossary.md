# Guía de la Nomenclatura de Desarrollo

## ¿Por qué es importante?

La nomenclatura es como un idioma común que todos hablamos en nuestro proyecto. Cuando todos usamos los mismos términos y convenciones, la comunicación y la colaboración se vuelven más efectivas. Además, esto facilita la integración de código de diferentes equipos y reduce la posibilidad de errores.

---

## Aspectos Clave

- **Idioma:** Toda la nomenclatura en inglés.
- **Clases y Objetos:** Nombres descriptivos y en singular en `UpperCamelCase` (por ejemplo: `UserProduct`).
- **Métodos y Funciones:** Nombres basados en verbos en `lowerCamelCase` (por ejemplo, `registerUser()`, `getProductList()`).
- **Rutas:** Utilizamos `kebab-case` (por ejemplo, `/inicio-sesion`, `/api/usuarios`).
- **Bases de Datos:** Nombres en plural para tablas y `snake_case` para columnas (por ejemplo, `users`, `user_name`).
- **Formato JSON:** Propiedades en minúsculas y `snake_case` en las solicitudes y respuestas JSON (por ejemplo, `user_name`, `product_price`).

---

## Nomenclatura General

### Clases y Objetos
- Utiliza nombres descriptivos y en singular para las clases y objetos.
- Usa `UpperCamelCase` para los nombres (e.g., `PaymentMethod`, `UserProduct`, `OrderUser`).

### Atributos
- Utiliza nombres concisos y descriptivos en minúsculas.
- Usa `snake_case` para separar palabras (por ejemplo, `user_name`, `product_price`).
- Evita prefijos o sufijos innecesarios en los nombres.

### Métodos y Funciones
- Usa nombres basados en verbos que describan la acción que realizan.
- Sigue la convención de `lowerCamelCase` (e.g., `registerUser()`, `getProductList()`).

---

## Nomenclatura de Rutas y Endpoints API

### Mejores Prácticas
1. **Nombres descriptivos:** Representan la acción o recurso. Ejemplo:  
   `GET /api/users/{id}`
2. **Verb HTTP para acciones:**  
   - `POST` para creaciones.  
   - `GET` para lecturas.  
   - `PUT` para actualizaciones.  
   - `DELETE` para eliminaciones.
3. **Rutas anidadas:** Para identificar recursos relacionados. Ejemplo:  
   `GET /api/articles/{id}/commentaries`
4. **Evita verbos en la URL:** Usa verbos HTTP en lugar de incluirlos en la URL. Ejemplo incorrecto:  
   `GET /api/getUser/{id}`
5. **Plural para colecciones:** Usa nombres en plural para colecciones. Ejemplo: `/users`.

### Rutas en Frontend
- Usa rutas en minúsculas separadas por guiones (`kebab-case`). Ejemplo: `/user-profile/{id}`.

### Rutas en Backend
- Usa el mismo formato de `kebab-case`. Ejemplo: `/api/user-products`.

### Nombres de Controladores de Rutas
- Nombres en plural y descriptivos (e.g., `UsersController`, `ProductsController`).
- Funciones con nombres claros y descriptivos (e.g., `getUsers`, `createProduct`).

---

## Endpoints Consistentes

| URL                          | Método | Descripción                                  |
|------------------------------|--------|----------------------------------------------|
| `/api/register`              | POST   | Endpoint para el registro de nuevos usuarios. |
| `/api/login/{id}`            | POST   | Endpoint para el inicio de sesión.           |
| `/api/user-profile/{id}`     | GET    | Endpoint para obtener el perfil del usuario. |
| `/api/update-user/{id}`      | PUT    | Endpoint para actualizar la información del usuario. |
| `/api/reset-password/{id}`   | POST   | Endpoint para restablecer la contraseña.     |
| `/api/products/{id}`         | GET    | Endpoint para obtener la lista de productos. |
| `/api/product-details/{id}`  | GET    | Endpoint para obtener detalles del producto. |
| `/api/cart/{id}`             | GET    | Endpoint para obtener el carrito del usuario. |
| `/api/add-to-cart/{id}`      | POST   | Endpoint para agregar productos al carrito.  |
| `/api/checkout`              | POST   | Endpoint para procesar el pago.             |
| `/api/order-history`         | GET    | Endpoint para obtener el historial de pedidos.|

---

## Nomenclatura de Bases de Datos (SQL)

### Tablas
- Usa nombres en plural para reflejar entidades (e.g., `users`, `products`).
- Utiliza `snake_case` para los nombres (e.g., `order_details`).

### Columnas
- Usa nombres descriptivos y en `snake_case` (e.g., `user_name`, `product_price`).

### Claves Primarias y Foráneas
- Prefija las claves primarias con el nombre de la tabla (e.g., `user_id`).
- Nombres consistentes para claves foráneas (e.g., `product_id`).

---

## Formato JSON Request and Response

- Utiliza nombres en minúsculas y `snake_case` (e.g., `user_name`, `product_price`).

---

Esta nomenclatura nos ayudará a mantener el código ordenado y comprensible, facilitando la colaboración entre equipos. Si tienen preguntas o sugerencias, ¡no duden en compartirlas!

**¡Gracias por su compromiso y entusiasmo!**
