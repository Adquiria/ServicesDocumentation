

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
  "monedaMain": "string",
  "cambioAdquiria": true,
  "monedaCambioMain": 0,
  "monedaSecun": "string",
  "monedaCambioSecun": 0,
  "userCode": 0,
  "userName": "string",
  "userActive": true,
  "userRol": "string",
  "enti_Id": 0,
  "entidad": {
    "enti_Id": 0,
    "enti_Nombre": "string",
    "enti_ResponsableNombre": "string",
    "enti_ResponsableEmail": "string",
    "enti_ResponsableTelefono": "string",
    "enti_RutaLogo": "string",
    "enti_Direccion": "string",
    "enti_Rut": "string",
    "enti_RazonSocial": "string",
    "enti_Estado": true,
    "enti_TipoCambioAdquiria": true,
    "enti_ValorCambio": 0,
    "tiam_Id": 0,
    "tipoAmbiente": {
      "fechaCreacion": "2024-12-11T17:45:41.076Z",
      "fechaUltimaModificacion": "2024-12-11T17:45:41.076Z",
      "userCodeCreacion": 0,
      "usuarioCreacion": {
        "userCode": 0,
        "userNameService": "string",
        "userPasswordService": "string",
        "userActiveService": true,
        "rose_Id": 0,
        "rol": {
          "rose_Id": 0,
          "rose_Rol": "string",
          "rose_Estado": true,
          "fechaCreacion": "2024-12-11T17:45:41.076Z"
        },
        "enti_Id": 0,
        "entidad": "string",
        "userSaltPasswordService": "string",
        "userNameOneService": "string",
        "userLastNameService": "string",
        "userTelephoneService": "string",
        "userEmailService": "string",
        "useService": true,
        "changePassword": true,
        "idUserEdit": 0
      },
      "userCodeModificacion": 0,
      "usuarioModificacion": {
        "userCode": 0,
        "userNameService": "string",
        "userPasswordService": "string",
        "userActiveService": true,
        "rose_Id": 0,
        "rol": {
          "rose_Id": 0,
          "rose_Rol": "string",
          "rose_Estado": true,
          "fechaCreacion": "2024-12-11T17:45:41.076Z"
        },
        "enti_Id": 0,
        "entidad": "string",
        "userSaltPasswordService": "string",
        "userNameOneService": "string",
        "userLastNameService": "string",
        "userTelephoneService": "string",
        "userEmailService": "string",
        "useService": true,
        "changePassword": true,
        "idUserEdit": 0
      },
      "tiam_Id": 0,
      "tiam_Tipo": "string",
      "tiam_Estado": true,
      "tiam_Descripcion": "string"
    },
    "fechaCreacion": "2024-12-11T17:45:41.076Z",
    "fechaUltimaModificacion": "2024-12-11T17:45:41.076Z",
    "userCodeCreacion": 0,
    "usuarioCreacion": {
      "userCode": 0,
      "userNameService": "string",
      "userPasswordService": "string",
      "userActiveService": true,
      "rose_Id": 0,
      "rol": {
        "rose_Id": 0,
        "rose_Rol": "string",
        "rose_Estado": true,
        "fechaCreacion": "2024-12-11T17:45:41.076Z"
      },
      "enti_Id": 0,
      "entidad": "string",
      "userSaltPasswordService": "string",
      "userNameOneService": "string",
      "userLastNameService": "string",
      "userTelephoneService": "string",
      "userEmailService": "string",
      "useService": true,
      "changePassword": true,
      "idUserEdit": 0
    },
    "userCodeModificacion": 0,
    "usuarioModificacion": {
      "userCode": 0,
      "userNameService": "string",
      "userPasswordService": "string",
      "userActiveService": true,
      "rose_Id": 0,
      "rol": {
        "rose_Id": 0,
        "rose_Rol": "string",
        "rose_Estado": true,
        "fechaCreacion": "2024-12-11T17:45:41.076Z"
      },
      "enti_Id": 0,
      "entidad": "string",
      "userSaltPasswordService": "string",
      "userNameOneService": "string",
      "userLastNameService": "string",
      "userTelephoneService": "string",
      "userEmailService": "string",
      "useService": true,
      "changePassword": true,
      "idUserEdit": 0
    }
  },
  "userToken": {
    "token": "string",
    "expiration": "2024-12-11T17:45:41.076Z"
  },
  "changePassword": true,
  "userNameInfo": "string"
}
```
## Diagra del objeto JSON
A continuacion, para mayor comprensión se grafica el anterior objeto JSON y sus niveles de anidamiento
![Untitled-2024-12-11-21-37-52](https://github.com/user-attachments/assets/0eb954b3-16a8-4f1b-b2fe-3d7dfbca9072)
