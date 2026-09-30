# rendex-app

Página puente **pública** para compartir **Rendex**, el asistente de
rentabilidad de freído de Alianza (Team Foods).

**Enlace para compartir:** https://juanortega-ts.github.io/rendex-app/

## Por qué existe

La aplicación real es una web app de Google Apps Script
(`juanortega-TS/rendex-gas`, privado). Al compartir su dirección `/exec`,
WhatsApp y similares la visitan sin sesión, terminan en el inicio de
sesión de Microsoft (el SSO de alianzateam.com) y muestran ese logo con
"Iniciar sesión en la cuenta".

Esta página tiene las etiquetas de vista previa (Open Graph) con el nombre
y la imagen de Rendex, y lleva a las personas a `/exec` con JavaScript.
Los robots de vista previa no ejecutan JavaScript, así que se quedan aquí.

## Seguridad

No contiene datos. Solo expone la dirección `/exec`, que igual exige
cuenta de alianzateam.com y estar en la lista de acceso de Rendex.
No guardar aquí nada más.

## Archivos

- `index.html`: etiquetas de vista previa y salto a `/exec`. Si cambia el
  ID de la implementación publicada, actualizarlo aquí (dos lugares).
- `vista-previa.png` (1200×630): símbolo sobre el fondo de marca #07272D,
  para que se vean las tres gotas.

WhatsApp guarda las vistas previas por dirección: si se cambia la imagen o
el texto, los mensajes ya enviados no se actualizan.
