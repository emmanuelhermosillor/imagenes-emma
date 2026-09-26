# Marca

`logo-emma.svg` — el logotipo secundario, el wordmark **em_ma**.

Sale de `EH - LOGOTIPO - SEC.V2.svg` del banco de identidad en Drive, con dos
cambios para la web:

- El relleno fijo `#efefef` pasa a **`currentColor`**. Así el mismo archivo
  sirve en modo claro y oscuro sin duplicarlo ni tocarlo desde JavaScript:
  hereda el color del texto de alrededor.
- La clase interna `.cls-1` —el nombre por defecto de Illustrator— pasa a
  `.logo-t`, para que no choque con cualquier otro SVG que se meta en línea en
  la misma página.

Va **en línea** en el HTML, no como `<img>`: un `<img>` no hereda
`currentColor`. Lleva `role="img"` y `aria-label="em_ma"`, y la página tiene
además un `<h1>` oculto con el nombre completo, porque un SVG no es un
encabezado.

viewBox 213.88 × 36.24. En el sitio se muestra a 88% del ancho en teléfono
—unos 343×58— y a 520px en escritorio.
