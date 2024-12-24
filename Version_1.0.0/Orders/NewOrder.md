## Request

### Endpoint base:

```http
https://adquiria-admin-api-etf7c0ayhccxeahp.centralus-01.azurewebsites.net
```

### Endpoint path:

```http
/api/Order/NewOrder
```

### Metodo:
```http
POST
```

### Descripción

Este servicio API permite gestionar la creación de pedidos.

## Bearer Token
El bearer token se obtiene como respuesta a tu solicitud de inicio de sesión a través de la API Login. Es necesario especificar ese bearer token obtenido previamente en el encabezado de esta request.

### Estructura del Objeto JSON

```json
{
  "usua_Cod": 0,
  "infoPago": {
    "mone_Id": 0,
    "installments": 0,
    "captureDataIframe": true,
    "paymentMethodId": "string",
    "tokenPayment": "string",
    "nombreCompletoPago": "string",
    "documento": "string",
    "tipoDocumento": "string",
    "email": "string",
    "coge_Id_Pago": 0,
    "mepa_Id": 0
  },
  "productosPedido": [
    {
      "idProducto": 0,
      "esRegalo": true,
      "cantidadEsRegalo": 0,
      "terminosSeleccionados": "string",
      "cantidad": 0
    }
  ],
  "entregaUsuario": {
    "sucu_Id": 0,
    "personaRetiro": "string",
    "direccionId": 0,
    "coes_Id_Logistica": 0,
    "coma_Id": 0
  },
  "facturacionPedido": {
    "nombres": "string",
    "apellidos": "string",
    "tipoDocumento": "string",
    "numeroDocumento": "string",
    "telefono": "string",
    "indicativo": "string",
    "rut": true,
    "razonSocial": "string",
    "numRut": "string",
    "idPais": 0
  },
  "codigoCupon": "string",
  "infoExtra": "string",
  "mone_Id": 0,
  "origen": "string"
}
```

### Descripción de Campos

#### Información del Pedido

- **usua_Cod** (entero): Código del usuario que realiza el pedido.

#### Información del Pago

- **infoPago** (objeto): Información relacionada con el pago del pedido.
    - **mone_Id** (entero): Identificador de la moneda utilizada.
    - **installments** (entero): Número de cuotas para el pago.
    - **captureDataIframe** (booleano): Indica si la captura de datos se realiza mediante un iframe.
    - **paymentMethodId** (cadena): Identificador del método de pago.
    - **tokenPayment** (cadena): Token de pago.
    - **nombreCompletoPago** (cadena): Nombre completo del titular del pago.
    - **documento** (cadena): Documento de identificación del titular del pago.
    - **tipoDocumento** (cadena): Tipo de documento de identificación.
    - **email** (cadena): Correo electrónico del titular del pago.
    - **coge_Id_Pago** (entero): Identificador del concepto de pago.
    - **mepa_Id** (entero): Identificador del medio de pago.

#### Productos del Pedido

- **productosPedido** (lista de objetos): Lista de productos incluidos en el pedido.
    - **idProducto** (entero): Identificador del producto.
    - **esRegalo** (booleano): Indica si el producto es un regalo.
    - **cantidadEsRegalo** (entero): Cantidad de productos que son regalos.
    - **terminosSeleccionados** (cadena): Términos seleccionados para el producto.
    - **cantidad** (entero): Cantidad del producto.

#### Entrega del Usuario

- **entregaUsuario** (objeto): Información relacionada con la entrega del pedido al usuario.
    - **sucu_Id** (entero): Identificador de la sucursal de entrega.
    - **personaRetiro** (cadena): Nombre de la persona que retira el pedido.
    - **direccionId** (entero): Identificador de la dirección de entrega.
    - **coes_Id_Logistica** (entero): Identificador del método de logística.
    - **coma_Id** (entero): Identificador del método de entrega.

#### Facturación del Pedido

- **facturacionPedido** (objeto): Información de facturación del pedido.
    - **nombres** (cadena): Nombres del titular de la factura.
    - **apellidos** (cadena): Apellidos del titular de la factura.
    - **tipoDocumento** (cadena): Tipo de documento de identificación.
    - **numeroDocumento** (cadena): Número de documento de identificación.
    - **telefono** (cadena): Teléfono del titular de la factura.
    - **indicativo** (cadena): Indicativo del teléfono.
    - **rut** (booleano): Indica si el titular tiene RUT.
    - **razonSocial** (cadena): Razón social del titular de la factura.
    - **numRut** (cadena): Número de RUT.
    - **idPais** (entero): Identificador del país.

#### Información Adicional

- **codigoCupon** (cadena): Código de cupón aplicado al pedido.
- **infoExtra** (cadena): Información adicional del pedido.
- **mone_Id** (entero): Identificador de la moneda utilizada.
- **origen** (cadena): Origen del pedido.

## Response
Si el `request` es correcto debe retornar:

```
Code: 200
Descripcion: Success
```

### Estructura del objeto JSON de respuestas
```json
{
  "orderResponse": {
    "success": true,
    "message": "string"
  },
  "peus_Id": 0
}
```
### Diagrama de datos JSON
![NewOrder-2024-12-12-23-20-26](https://github.com/user-attachments/assets/7c8fa01a-6673-44a4-a917-78fe241861ce)

