# Mr. Robot — Omarchy theme

Tema oscuro de alto contraste con tono de terminal, vigilancia y glitch:
negro profundo, blanco de fósforo y rojo de alerta. Está creado desde cero
para Omarchy e incluye fondos originales y fondos seleccionados para uso
personal.

## Instalación directa con Omarchy

```bash
omarchy theme install \
  https://github.com/ciprianotoor/omarchy-mr-robot-theme.git
```

Omarchy clonará este repositorio directamente en
`~/.config/omarchy/themes/mr-robot` y activará el tema.

Para cambiar entre los fondos incluidos:

```bash
omarchy theme bg next
```

### Desarrollo local

Si trabajas con una copia local del tema:

```bash
mkdir -p ~/.config/omarchy/themes
ln -sfn "$PWD" ~/.config/omarchy/themes/mr-robot
omarchy theme set mr-robot
```

Este repositorio contiene únicamente el tema. La configuración completa de
dotfiles está en el repositorio principal:
`DotfileArchOmarchyCipriano`.

## Inspiración visual

- Fondo casi negro y tipografía clara de terminal.
- Rojo `#F2293A` para alertas, bordes y estados críticos.
- Blanco fósforo `#E7E9E7` para lectura prolongada.
- Gris CRT y líneas de interferencia para la sensación de monitor antiguo.
- Fondos SVG y JPG incluidos directamente en `backgrounds/`.

`preview.png` es la miniatura del tema. `backgrounds/mr-robot-ascii.png` es
el fondo ASCII rojo/negro que Omarchy puede incluir al usar `theme bg next`.

## Licencia

Las configuraciones, documentación y fondos creados localmente por el autor
se distribuyen bajo la licencia MIT del repositorio raíz. La MIT no cubre los
JPG de terceros, frases, personajes, marcas ni logotipos relacionados con
Mr. Robot. Consulta [`SOURCES.txt`](backgrounds/SOURCES.txt) y verifica las
condiciones de cada fuente antes de redistribuir o usar comercialmente esos
fondos.

Este tema no está afiliado, patrocinado ni aprobado por Omarchy, Arch Linux,
los titulares de derechos de Mr. Robot ni los autores de los recursos
externos.

El tema se proporciona “tal cual”. Haz copias de seguridad antes de enlazarlo
y adapta las rutas o comandos si tu instalación de Omarchy difiere.
