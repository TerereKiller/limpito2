# Limpito · Ventas y costos

Página web de un solo archivo (`index.html`), sin instalar nada ni depender de internet.

## Secciones
- **Ventas:** una venta puede llevar varios productos. Buscás el producto escribiendo, ponés cantidad y Enter, y repetís. Se registra con cliente/nota y fecha. Podés buscar ventas por cliente o producto y filtrar por mes.
- **Productos:** nombre y precio de venta, con costo, ganancia, margen y stock de cada uno.
- **Recetas:** los insumos de cada producto por unidad vendida, con el costo de cada uno y su % del total. Calcula el precio sugerido para el margen que elijas y permite preparar un lote.
- **Inventario:** stock de materias primas y de productos terminados, con aviso de stock bajo y botón para registrar compras.
- **Materias primas:** precios de todo lo que suma al costo (insumos, botellas, tapas, stickers).
- **Resumen:** ventas, costo y ganancia mes a mes, con gráfico y ventas por producto.

## Cómo funciona el stock
1. **Materias primas:** en *Inventario → Ajustar* cargás lo que tenés hoy. Con *Registrar compra* sumás lo que comprás (y actualiza el precio).
2. **Producción:** en *Recetas → Preparar un lote* ponés cuántas unidades hacés y tocás *Registrar producción*. Descuenta los insumos y suma los productos terminados.
3. **Ventas:** cada venta descuenta del stock del producto. Si borrás o editás una venta, el stock se corrige.
4. Los ítems que dicen **"Sin controlar"** no se descuentan hasta que cargues su stock con *Ajustar*. Así podés empezar de a poco.

## Usarla
Abrí `index.html` en el navegador. Los datos se guardan automáticamente **en ese navegador y en ese dispositivo**.

Si ya usabas la versión anterior en el mismo navegador y desde la misma dirección, tus datos se actualizan solos. Las ventas cargadas por separado para un mismo cliente y fecha se unen en una sola venta con varios productos. Además se guarda una copia de seguridad de tus datos viejos dentro del navegador.

## Publicarla en GitHub (GitHub Pages)
1. Subí `index.html` y este `README.md` a tu repositorio (reemplazando los anteriores).
2. En el repo: Settings → Pages → Source: *Deploy from a branch* → rama `main`, carpeta `/ (root)` → Save.
3. En un minuto queda en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

GitHub Pages es gratis solo con repositorios **públicos**. Si usás una dirección nueva, el navegador la ve como otro sitio y empieza vacío: restaurá tu respaldo ahí.

## Importante: dónde quedan tus datos
GitHub guarda el **código** de la página, no lo que cargás en ella. Los datos viven en el navegador.
1. Tocá **Descargar respaldo** cada tanto (una vez por semana). La página te avisa si pasaron 7 días.
2. Para pasar los datos a otro navegador o dispositivo, o recuperarlos, usá **Restaurar respaldo**.
3. **No subas los respaldos `.json` a un repositorio público**: cualquiera vería tus precios, costos y ventas. Guardalos en un repositorio privado aparte, en tu computadora o en tu Drive.
