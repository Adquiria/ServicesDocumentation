
## Request


### Endpoint base:

```http
https://adquiria-admin-api-etf7c0ayhccxeahp.centralus-01.azurewebsites.net
```

### Endpoint path:

```http
/api/Pro_Atributos/NewTerminoAtributo
```

### Metodo:

```http
POST
```

### Descripción

Este servicio API permite la creación de términos de atributos.


### Bearer Token
El bearer token se obtiene como respuesta a tu solicitud de inicio de sesión a través de la API **Login**. Es necesario especificar ese bearer token obtenido previamente en el encabezado de esta request.

### Estructura del Objeto JSON

```json
{
  "id": 0,
  "atpr_Id": 0,
  "nombre": "string",
  "imagen": "string",
  "tipoImagen": "string",
  "estado": true
}
```

### Descripción de Campos

#### Información del Atributo

- **id** (entero): Identificador único del atributo.
- **atpr_Id** (entero): Identificador del atributo principal asociado.
- **nombre** (cadena): Nombre del atributo.
- **imagen** (cadena): URL de la imagen asociada al atributo.
- **tipoImagen** (cadena): Tipo de imagen (ej. jpeg, png).
- **estado** (booleano): Estado del atributo (activo/inactivo).

## Response
Si el `request` es correcto debe retornar:

```
Code: 200
Descripcion: Success
```

