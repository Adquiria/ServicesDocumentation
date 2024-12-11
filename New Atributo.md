
## Request

### Endpoint base:

```HTTP
https://adquiria-admin-api-etf7c0ayhccxeahp.centralus-01.azurewebsites.net
```

### Endpoint path:

```http
/api/Pro_Atributos/NewAtributo
```

### Metodo:

```HTTP
POST
```



### Descripción

Este servicio API permite la gestión de la creación de terminos.


### Bearer Token
El bearer token se obtiene como respuesta a tu solicitud de inicio de sesión a través de la API **Login**. Es necesario especificar ese bearer token obtenido previamente en el encabezado de esta request.

### Estructura del Objeto JSON

```json
{
  "userCodeCreacion": 0,
  "userCodeUltimaModificacion": 0,
  "id": 0,
  "tipo": "string",
  "muchosTerminos": true,
  "estado": true,
  "muat_Id": 0,
  "enti_Id": 0
}
```

### Descripción de Campos

#### Información del Término

- **userCodeCreacion** (entero): Código del usuario que creó el término.
- **userCodeUltimaModificacion** (entero): Código del usuario que realizó la última modificación.
- **id** (entero): Identificador único del término.
- **tipo** (cadena): Tipo del término.
- **muchosTerminos** (booleano): Indica si el término se asocia con múltiples términos.
- **estado** (booleano): Estado del término (activo/inactivo).
- **muat_Id** (entero): Identificador de la categoría o grupo asociado al término.
- **enti_Id** (entero): Identificador de la entidad propietaria del término.

## Response
Si el `request` es correcto debe retornar:

```
Code: 200
Descripcion: Success
```

