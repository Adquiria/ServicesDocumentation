## Request

### Endpoint base:

```HTTP
https://adquiria-admin-api-etf7c0ayhccxeahp.centralus-01.azurewebsites.net
```

### Endpoint path:

```http
/api/Pro_Categorias/NewCategoriasProductos
```

### Metodo:

```HTTP
POST
```


### Descripción

Este servicio API permite la creación de categorías y de su información relacionada con las.


### Bearer Token
El bearer token se obtiene como respuesta a tu solicitud de inicio de sesión a través de la API **Login**. Es necesario especificar ese bearer token obtenido previamente en el encabezado de esta request.

### Estructura del Objeto JSON



```json
{
  "id": 0,
  "nombre": "string",
  "estado": true,
  "capo_IdPadre": 0,
  "esCategoriaPrincipal": true,
  "enti_Id": 0
}
```

### Descripción de Campos

#### Información de la Categoría

- **id** (entero): Identificador único de la categoría. se manda vacío cuando se crea la categoría, el sistemas agrega el id automáticamente
- **nombre** (cadena): Nombre de la categoría.
- **estado** (booleano): Estado de la categoría (activo/inactivo).
- **capo_IdPadre** (entero): Identificador de la categoría padre, si aplica, si por el contrario quire crear una categoria padre ese campo debe tener el valor = `null`.
- **esCategoriaPrincipal** (booleano): Indica si la categoría es principal.
- **enti_Id** (entero): Identificador de la entidad propietaria de la categoría.

## Response
Si el `request` es correcto debe retornar:

```
Code: 200
Descripcion: Success
```
```json
{
   "success": true,
   "message": "El arbol de categorías se agrego con éxito"
}
```

