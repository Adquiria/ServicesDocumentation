

## Request

### Endpoint base:

```HTTP
https://adquiria-admin-api-etf7c0ayhccxeahp.centralus-01.azurewebsites.net
```

### Endpoint path:

```http
/api/Pro_Caracteristicas/NewCaracteriscaCompleta
```

### Metodo:

```HTTP
POST
```



### Descripción

Este servicio API permite la gestión de características, incluyendo la creación y de información relacionada con características y sus características hijas.


### Bearer Token
El bearer token se obtiene como respuesta a tu solicitud de inicio de sesión a través de la API **Login**. Es necesario especificar ese bearer token obtenido previamente en el encabezado de esta request.

### Estructura del Objeto JSON

```json
{
  "userCodeCreacion": 0,
  "userCodeUltimaModificacion": 0,
  "id": 0,
  "nombre": "string",
  "estado": true,
  "enti_Id": 0,
  "caracteristicasHijas": [
    {
      "id": 0,
      "nombre": "string"
    }
  ]
}
```

### Descripción de Campos

#### Información de la Característica

- **userCodeCreacion** (entero): Código del usuario que creó la característica.
- **userCodeUltimaModificacion** (entero): Código del usuario que realizó la última modificación.
- **id** (entero): Identificador único de la característica.
- **nombre** (cadena): Nombre de la característica.
- **estado** (booleano): Estado de la característica (activo/inactivo).
- **enti_Id** (entero): Identificador de la entidad propietaria de la característica.
- **caracteristicasHijas** (lista de objetos): Lista de características hijas asociadas.
    - **id** (entero): Identificador de la característica hija.
    - **nombre** (cadena): Nombre de la característica hija.

## Response
Si el `request` es correcto debe retornar:

```
Code: 200
Descripcion: Success
```
