# S.R. ACOBAMBA

**Sistema de punto de venta (POS) de la tienda Super Remates Acobamba.**
Versión personalizada de SRZ VENTAS, desarrollada por **Grupo Salazar**.

Versión: 2.0.1+4 · Hecho con Flutter · Android y iPhone · Funciona 100 % en el celular, sin servidor.

---

## ¿Qué es?

S.R. ACOBAMBA es la app de ventas de **Super Remates Acobamba**. Es una versión de SRZ VENTAS con la marca de la tienda: nombre, icono, pantalla de inicio y colores **celeste y rosado**.

Se instala como una app aparte (identificador `com.sracobamba`), así que puede convivir en el mismo celular con SRZ VENTAS sin reemplazarla.

## ¿Para qué sirve?

- Registrar las ventas de la tienda desde el celular.
- Controlar el inventario (TV y electrónica, celulares y accesorios, juguetes, hogar y cocina, ropa y más).
- Cobrar en efectivo, Yape, Plin o tarjeta, y calcular el vuelto.
- Imprimir el ticket o enviarlo por WhatsApp.
- Revisar el historial de ventas y sacar reportes en Excel.

## Funciones principales

**Ventas**
- Escáner de códigos de barras con la cámara.
- Venta por unidad o por peso.
- Descuento en **soles (S/)** o en **porcentaje (%)**.
- Métodos de pago: Efectivo, Yape, Plin y Tarjeta, con QR de Yape/Plin.
- Monto recibido, botones rápidos y **vuelto** automático.
- Nota opcional por venta.

**Productos e inventario**
- Productos con foto, precios, stock y categoría.
- Tallas y colores (útil para ropa y calzado), tamaños y opciones con precio extra.
- Generación y exportación de códigos de barras (imagen y PDF).

**Tickets e impresión**
- Impresora térmica **Bluetooth** (58 mm u 80 mm).
- Ticket con nombre, dirección, teléfono, RUC y mensaje de la tienda.
- Compartir el ticket por WhatsApp.

**Control**
- Historial de ventas y exportación a Excel.
- Vendedores y categorías.
- **Respaldo** completo e importación.
- Moneda configurable (por defecto S/).

## Cómo funciona

1. Al abrir la app se ve el logo animado de S.R. ACOBAMBA.
2. La primera vez aparece la bienvenida con el botón **Empezar** y se configuran los datos de la tienda.
3. En **Ajustes** se configura la impresora, los métodos de pago, los QR y los vendedores.
4. En **Inventario** se cargan los productos.
5. Para vender: escanear o elegir productos, revisar la orden, aplicar descuento si hace falta, elegir el método de pago y confirmar. El stock baja solo y la venta queda en el historial.

Los datos se guardan **en el celular**. Esta versión tiene su propia base de datos: para pasar productos desde SRZ VENTAS, hay que hacer un **respaldo** allá e importarlo aquí (Ajustes → Avanzado). Conviene hacer respaldos seguido.

## Importante

Los tickets son comprobantes simples de venta. **No son boletas ni facturas** ni documentos vinculados a SUNAT.

## Compilar

```bash
flutter pub get
flutter run
flutter build apk --release
```

Para Android release se necesita `android/key.properties` y el archivo `.jks` (no se suben al repositorio). Para iPhone se puede usar Codemagic (`codemagic.yaml`, bundle ID `com.sracobamba`).

## Créditos

Sistema desarrollado por **Grupo Salazar**.
Soporte por WhatsApp: **+51 900 725 974**

Tienda: **Super Remates Acobamba** — "Variedad, calidad y los mejores precios".
