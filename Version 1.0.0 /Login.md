

## Request

### Endpoint base:

```HTTP
https://adquiria-admin-api-etf7c0ayhccxeahp.centralus-01.azurewebsites.net
```

### Endpoint path:

```http
/api/Account/Login
```

### Metodo:

```HTTP
POST
```


### Descripción

Este servicio API permite la gestión de la autenticación para obtener las credenciales asociadas a las acciones dentro de la plataforma

### Estructura del Objeto JSON

```json
{
  "user": "string",
  "password": "string",
  "enti_Id": 0 -> ESTE IDENTIFICADOR DEBE SOLICITARCE A SOPORTE ADQUIRIA
}
```

### Descripción de Campos

#### Información del Usuario

- **user** (cadena): Nombre de usuario.
- **password** (cadena): Contraseña del usuario.
- **enti_Id** (entero): Identificador de la entidad asociada al usuario.

## Response
Si el `request` es correcto debe retornar:

```
Code: 200
Descripcion: Success
```

y la estructura del siguiente JSON:
```json
{
  "userCode": 0,
  "userName": "string",
  "userActive": true,
  "userRol": "string",
  "enti_Id": 0,
  "entidad": {
    "enti_Id": 0,
    "enti_Nombre": "string",
    "enti_ResponsableNombre": "string",
    "enti_ResponsableEmail": "string@email.com",
    "enti_ResponsableTelefono": "+57 0000000000",
    "enti_RutaLogo": "https://[...].PNG",
    "enti_Direccion": "string",
    "enti_Rut": "string",
    "enti_RazonSocial": "string",
    "enti_Estado": true,
    "enti_TipoCambioAdquiria": true,
    "enti_ValorCambio": 0,
    "tiam_Id": 0,
    "tipoAmbiente": null,
    "fechaCreacion": "2024-06-27T02:19:41.985",
    "fechaUltimaModificacion": "2024-12-11T16:21:47.861719",
    "userCodeCreacion": 0,
    "usuarioCreacion": null,
    "userCodeModificacion": 0,
    "usuarioModificacion": null
  },
  "userToken": {
    "token": "eyJh[...]0gEU",
    "expiration": "2024-12-12T04:03:02.8244278Z"
  },
  "changePassword": true,
  "userNameInfo": "string",
  "monedaMain": "USD",
  "cambioAdquiria": true,
  "monedaCambioMain": 0,
  "monedaSecun": "UYU",
  "monedaCambioSecun": 44.95
}
```
## Diagra del objeto JSON
A continuacion, para mayor comprensión se grafica el anterior objeto JSON y sus niveles de anidamiento
![Login Return JSON-2024-12-12-00-34-03](https://github.com/user-attachments/assets/c1a8a3b3-1051-4c18-9afc-a4f51bb97115)

