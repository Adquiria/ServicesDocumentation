
## Request

### Endpoint base:

```HTTP
https://adquiria-admin-api-etf7c0ayhccxeahp.centralus-01.azurewebsites.net
```

### Endpoint path:

```http
/api/Pro_Cocardas/NewCocarda
```

### Metodo:

```HTTP
POST
```



### Descripción

Este servicio API permite la gestión de la creación de cocardas.

### Bearer Token
El bearer token se obtiene como respuesta a tu solicitud de inicio de sesión a través de la API **Login**. Es necesario especificar ese bearer token obtenido previamente en el encabezado de esta request.

### Estructura del Objeto JSON

```json
{
  "userCodeCreacion": 0,
  "userCodeUltimaModificacion": 0,
  "id": 0,
  "enti_Id": 0,
  "nombre": "string",
  "imagen": "string",
  "tipoImagen": "string",
  "type": "string",
  "infoTexto": "string",
  "ubicacion": "string",
  "px": "string",
  "estado": true
}
```

### Descripción de Campos

#### Información del Elemento

- **userCodeCreacion** (entero): Código del usuario que creó el elemento.
- **userCodeUltimaModificacion** (entero): Código del usuario que realizó la última modificación.
- **id** (entero): Identificador único del elemento.
- **enti_Id** (entero): Identificador de la entidad propietaria del elemento.
- **nombre** (cadena): Nombre del elemento.
- **imagen** (cadena): URL de la imagen asociada al elemento.
- **tipoImagen** (cadena): Tipo de imagen (ej. jpeg, png).
- **type** (cadena): Tipo del elemento.
- **infoTexto** (cadena): Información textual adicional del elemento.
- **ubicacion** (cadena): Ubicación asociada al elemento.
- **px** (cadena): Coordenadas en formato px del elemento.
- **estado**

## Response
Si el `request` es correcto debe retornar:

```
Code: 200
Descripcion: Success
```
