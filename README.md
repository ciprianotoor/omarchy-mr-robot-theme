# Mr. Robot — Omarchy theme

Tema oscuro de alto contraste con tono de terminal, vigilancia y glitch:
negro profundo, blanco de fósforo y rojo de alerta. Está creado desde cero
para Omarchy. Es un tema comunitario/no oficial e incluye recursos originales
y recursos de terceros cuya licencia debe revisarse por separado.

> Si eres nuevo en Omarchy: este repositorio instala únicamente un tema. No
> instala Arch Linux, Omarchy, aplicaciones, fuentes ni el repositorio completo
> de dotfiles. Haz una copia de seguridad antes de cambiar tu tema.

## Instalación directa con Omarchy

```bash
omarchy theme install \
  https://github.com/ciprianotoor/omarchy-mr-robot-theme.git
```

Omarchy clonará este repositorio directamente en
`~/.config/omarchy/themes/mr-robot` y activará el tema.

El comando crea una copia Git independiente del repositorio de dotfiles. No
uses también un enlace simbólico con el mismo nombre, porque una instalación
puede reemplazar o dejar confusa la otra.

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

### Actualizar o quitar

Para actualizar la copia instalada, usa el menú `temasync` del repositorio de
dotfiles o, desde la carpeta instalada, ejecuta `git pull --ff-only` y después:

```bash
omarchy theme refresh
```

Para quitarlo, activa primero otro tema y comprueba la ruta antes de borrar:

```bash
omarchy theme set <otro-tema>
ls -ld ~/.config/omarchy/themes/mr-robot
```

No borres `~/.local/share/omarchy/`; esa carpeta pertenece a la instalación de
Omarchy y no a este tema.

## Inspiración visual

- Fondo casi negro y tipografía clara de terminal.
- Rojo `#F2293A` para alertas, bordes y estados críticos.
- Blanco fósforo `#E7E9E7` para lectura prolongada.
- Gris CRT y líneas de interferencia para la sensación de monitor antiguo.
- Fondos SVG y JPG incluidos directamente en `backgrounds/`.

`preview.png` es la miniatura del tema. `backgrounds/mr-robot-ascii.png` es
el fondo ASCII rojo/negro que Omarchy puede incluir al usar `theme bg next`.

## Licencia, recursos de terceros y límites

Esta sección es informativa y no constituye asesoría legal. La licencia MIT de
este repositorio cubre únicamente las configuraciones, scripts, documentación
y recursos originales creados por el autor, salvo indicación distinta.

Los JPG de terceros están identificados o referenciados en
[`SOURCES.txt`](backgrounds/SOURCES.txt). Sus derechos, permisos, atribución y
restricciones pertenecen a sus respectivos autores o sitios de origen. MIT no
te concede derechos sobre esos JPG, ni sobre frases, personajes, marcas,
logotipos o material promocional de *Mr. Robot*. Verifica cada fuente antes de
redistribuir el repositorio o usar los recursos comercialmente; si no puedes
verificar los permisos, elimina los archivos de terceros de tu copia.

Arch Linux, Omarchy, Hyprland, fuentes, iconos, plugins y demás dependencias
también conservan sus propias licencias. Revisa sus términos por separado.

Este tema no está afiliado, patrocinado ni aprobado por Omarchy, Arch Linux,
los titulares de derechos de Mr. Robot ni los autores de los recursos
externos.

“Mr. Robot” se usa solamente para describir la inspiración visual de este
proyecto de fans. No se permite presentar el tema como oficial, autorizado o
respaldado por los titulares de la serie o por Omarchy.

El tema se proporciona “tal cual”, sin garantía de compatibilidad, seguridad o
ausencia de errores. El usuario es responsable de revisar los archivos,
mantener copias de seguridad y cumplir las licencias y leyes aplicables.
