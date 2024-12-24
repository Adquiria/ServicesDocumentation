## Request

### Endpoint base:

```HTTP
https://adquiria-admin-api-etf7c0ayhccxeahp.centralus-01.azurewebsites.net
```

### Endpoint path:

```http
/api/Pro_GuiasTalles/ListGuiasTalles/{enti_Id}
```

### Metodo:

```HTTP
GET
```


### Descripción

Este servicio API permite listar todas las Guias Talles de producto que se guardaron previamente


### Bearer Token
El bearer token se obtiene como respuesta a tu solicitud de inicio de sesión a través de la API **Login**. Es necesario especificar ese bearer token obtenido previamente en el encabezado de esta request.

### Estructura del Objeto JSON
para esta petición se manda por `` URL `` el Identificador de la entidad `` {enti_Id} `` Dicho identificador debe se obtiene cuando se realiza el login.
