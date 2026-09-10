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

## Fotos

Las fotos reales de Kenay están en `./img` (`01-saludo`, `02/03-chiste`, `prod-02..prod-20`).
Para cambiarlas, reemplazá los archivos con los mismos nombres, o editá las rutas en el
bloque `DATOS DE FOTOS` del `<script>`.

- **ANTES**: todo mezclado en una sola "Cámara" (fotos reales + relleno para dar volumen).
- **DESPUÉS**: el sistema deja la carpeta "Estados Kenay" con 20 piezas ordenadas
  (buen día · 2 chistes · 16 productos · cierre) y un botón "Seleccionar las 20".
- El **cierre** es una placa generada (gradiente + ▶). Para usar un video/enlace real,
  cambiá `CIERRE` por `{ img:'img/cierre.jpg', label:'Cierre', link:'https://...' }`.

## Aviso

Demo con fines de demostración comercial. No es la aplicación real de WhatsApp ni
está afiliada a WhatsApp LLC / Meta Platforms.
