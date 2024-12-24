
## Request

### Endpoint base:

```HTTP
https://adquiria-admin-api-etf7c0ayhccxeahp.centralus-01.azurewebsites.net
```

### Endpoint path:

```http
/api/Pro_Marcas/NewMarca
```

### Metodo:

```HTTP
POST
```


### Descripción

Este servicio API permite la gestión de diversos elementos, incluyendo la creación de una marca de producto y de información relevante para la misma, como una imagen de la misma.


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
  "type": "string",
  "estado": true,
  "enti_Id": 0
}
```

### Descripción de Campos

#### Información del Elemento

- **userCodeCreacion** (OBLIGATORIO) (entero): Código del usuario que creó el elemento.
- **userCodeUltimaModificacion** (OBLIGATORIO) (entero): Código del usuario que realizó la última modificación.
- **id** (entero): Identificador único del elemento.
- **nombre** OBLIGATORIO (cadena): Nombre del elemento.
- **imagen** (cadena): URL de la imagen asociada al elemento.
- **tipoImagen** (cadena): Tipo de imagen (ej. jpeg, png).
- **type** (cadena): Tipo del elemento.
- **estado** (OBLIGATORIO) (booleano): Estado del elemento (activo/inactivo).
- **enti_Id** (OBLIGATORIO) (entero): Identificador de la entidad propietaria del elemento.

## Response
Si el `request` es correcto debe retornar:

```
Code: 200
Descripcion: Success
```

### Objeto JSON
```JSON
{
   "success": true,
   "message": "La marca se agrego con éxito"
}
```
