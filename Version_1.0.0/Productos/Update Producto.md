## Request

### Endpoint base:

```HTTP
https://adquiria-admin-api-etf7c0ayhccxeahp.centralus-01.azurewebsites.net
```

### Endpoint path:

```HTTP
/api/Pro_Productos/UpdateProductos
```

### Metodo:

```HTTP
POST
```

### Descripción

Este servicio API permite la modificación de productos, incluyendo la información relacionada con el mismo, variantes, imágenes y detalles asociados.

### Bearer Token
El bearer token se obtiene como respuesta a tu solicitud de inicio de sesión a través de la API **Login**. Es necesario especificar ese bearer token obtenido previamente en el encabezado de esta request.

### Estructura del Objeto JSON

```JSON
{
  "userCodeCreacion": 0,
  "userCodeUltimaModificacion": 0,
  "id": 0,
  "enti_Id": 0,
  "mone_Id": 0,
  "nombre": "string",
  "descripcion": "string",
  "sku": "string",
  "productoSimple": true,
  "productoSimpleStock": 0,
  "precioSimple": true,
  "precioNormal": 0,
  "precioRebajado": 0,
  "imagenPrincipal": "string",
  "tipoImagen": "string",
  "estado": true,
  "fechaPublica": "2024-12-05T22:54:26.542Z",
  "imagenesProducto": [
    {
      "id": 0,
      "imagen": "string",
      "tipoImagen": "string"
    }
  ],
  "detalle": {
    "id": 0,
    "gupr_Id": 0,
    "mapr_Id": 0,
    "coca_Id": 0
  },
  "variantesPosibles": [
    {
      "atpr_Id": 0,
      "tege_Id_PosiblesTerminos": "string",
      "stock": 0,
      "skuPropio": "string",
      "precioPropio": 0,
      "precioRebajadoPropio": 0
    }
  ],
  "categoriasAsociadas": [
    0
  ],
  "caracteristicasAsociadas": [
    0
  ]
}
```

### Descripción de Campos

#### Información del Producto

- **userCodeCreacion** (entero): Código del usuario que creó el producto.
- **userCodeUltimaModificacion** (entero): Código del usuario que realizó la última modificación.
- **id** (entero): Identificador único del producto.
- **enti_Id** (entero): Identificador de la entidad propietaria del producto.
- **mone_Id** (entero): Identificador de la moneda en la cual se manejan los precios.
- **nombre** (cadena): Nombre del producto.
- **descripcion** (cadena): Descripción del producto.
- **sku** (cadena): Código SKU (Stock Keeping Unit) del producto.
- **productoSimple** (booleano): Indica si el producto es simple.
- **productoSimpleStock** (entero): Stock del producto simple.
- **precioSimple** (booleano): Indica si el precio es simple.
- **precioNormal** (decimal): Precio normal del producto.
- **precioRebajado** (decimal): Precio rebajado del producto.
- **imagenPrincipal** (cadena): URL de la imagen principal del producto.
- **tipoImagen** (cadena): Tipo de imagen principal (ej. jpeg, png).
- **estado** (booleano): Estado del producto (activo/inactivo).
- **fechaPublica** (datetime): Fecha y hora de publicación del producto.

#### Imágenes del Producto

- **imagenesProducto** (lista de objetos): Lista de imágenes asociadas al producto.
    - **id** (entero): Identificador de la imagen.
    - **imagen** (cadena): Imagen codificada en base64.
    - **tipoImagen** (cadena): Tipo de imagen (ej. jpeg, png).

#### Detalles del Producto

- **detalle** (objeto): Información detallada del producto.
    - **id** (entero): Identificador del detalle.
    - **gupr_Id** (entero): Identificador del grupo de productos.
    - **mapr_Id** (entero): Identificador del fabricante o proveedor.
    - **coca_Id** (entero): Identificador de la categoría.

#### Variantes Posibles

- **variantesPosibles** (lista de objetos): Lista de variantes posibles del producto.
    - **atpr_Id** (entero): Identificador del atributo del producto.
    - **tege_Id_PosiblesTerminos** (cadena): Términos posibles para la variante.
    - **stock** (entero): Stock de la variante.
    - **skuPropio** (cadena): SKU propio de la variante.
    - **precioPropio** (decimal): Precio propio de la variante.
    - **precioRebajadoPropio** (decimal): Precio rebajado propio de la variante.

#### Asociaciones

- **categoriasAsociadas** (lista de enteros): Identificadores de las categorías asociadas.
- **caracteristicasAsociadas** (lista de enteros): Identificadores de las características asociadas.

## Response
Si el `request` es correcto debe retornar:

```
Code: 200
Descripcion: Success
```
