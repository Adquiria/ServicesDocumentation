
## Request

### Endpoint base:

```HTTP
https://adquiria-admin-api-etf7c0ayhccxeahp.centralus-01.azurewebsites.net
```

### Endpoint path:

```http
/api/Pro_GuiasTalles/NewGuiaTalles
```

### Metodo:

```HTTP
POST
```



### Descripción

Este servicio API permite la creación de información de Talles, con un enfoque en la administración de imágenes, contenido HTML y estados.


### Bearer Token
El bearer token se obtiene como respuesta a tu solicitud de inicio de sesión a través de la API **Login**. Es necesario especificar ese bearer token obtenido previamente en el encabezado de esta request.

### Estructura del Objeto JSON

```json
{
  "userCodeCreacion": 0,
  "userCodeUltimaModificacion": 0,
  "id": 0,
  "nombre": "string",
  "imagen": "string",
  "tipoImagen": "string",
  "html": "string",
  "estado": true,
  "enti_Id": 0
}
```

### Descripción de Campos

#### Información del Elemento

- **userCodeCreacion** (entero): Código del usuario que creó el elemento.
- **userCodeUltimaModificacion** (entero): Código del usuario que realizó la última modificación.
- **id** (entero): Identificador único del elemento.
- **nombre** (cadena): Nombre del elemento.
- **imagen** (cadena): URL de la imagen asociada al elemento.
- **tipoImagen** (cadena): Tipo de imagen (ej. jpeg, png).
- **html** (cadena): Contenido HTML asociado al elemento.
- **estado** (booleano): Estado del elemento (activo/inactivo).
- **enti_Id** (entero): Identificador de la entidad propietaria del elemento.


## Response
Si el `request` es correcto debe retornar:

```
Code: 200
Descripcion: Success
```

