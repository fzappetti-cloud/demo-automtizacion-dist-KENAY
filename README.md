# Demo · Estados de WhatsApp para Distribuidora Kenay

Simulación interactiva de una sola página (`demo-estados-kenay.html`) para mostrar,
sin explicaciones, la diferencia entre subir el Estado de WhatsApp **como es hoy**
(buscar foto por foto entre carpetas desordenadas a las 3 AM) y **con el sistema**
(la carpeta "Estados Kenay" del día ya armada con las 5 piezas).

## Uso

Abrir `demo-estados-kenay.html` en cualquier navegador. No requiere build ni backend
(solo internet para la tipografía Google Fonts).

Para levantarlo con servidor local:

```bash
npx -y http-server -p 4173 -c-1
```

y entrar a `http://localhost:4173/demo-estados-kenay.html`.

## Reemplazar los placeholders por fotos reales

Las imágenes de producto son bloques de color + emoji. En el bloque `DATOS DE FOTOS`
del `<script>`, cambiar `{ emoji, label, bg }` por `{ label, img: 'ruta/o/url.jpg' }`.
`renderTile()` y `buildPreview()` ya soportan la propiedad `img`.

## Aviso

Demo con fines de demostración comercial. No es la aplicación real de WhatsApp ni
está afiliada a WhatsApp LLC / Meta Platforms.
