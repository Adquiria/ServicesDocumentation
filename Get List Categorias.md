## Request

### Endpoint base:

```HTTP
https://adquiria-admin-api-etf7c0ayhccxeahp.centralus-01.azurewebsites.net
```

### Endpoint path:

```http
/api/Pro_Categorias/GetListCategorias
```

### Metodo:

```HTTP
POST
```


### Descripción

Este servicio API permite la gestión de asociaciones de categorías con una entidad específica.

### Bearer Token
El bearer token se obtiene como respuesta a tu solicitud de inicio de sesión a través de la API **Login**. Es necesario especificar ese bearer token obtenido previamente en el encabezado de esta request.

### Estructura del Objeto JSON

```json
{
  "enti_Id": 0,
  "categoriasList": [
    0
  ]
}
```

### Descripción de Campos

#### Información de la Asociación de Categorías

- **enti_Id** (entero): Identificador de la entidad propietaria. null para obtener todas las categrias
- **categoriasList** (lista de enteros): Lista de identificadores de las categorías asociadas.

## Response
Si el `request` es correcto debe retornar:

```
Code: 200
Descripcion: Success
```

