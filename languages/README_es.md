# vkt-note

[English](../README.md) | [中文](README_zh.md) | [Deutsch](README_de.md) | Español | [日本語](README_ja.md) | [Français](README_fr.md)

Manual de usuario oficial · Una extensión ligera de notas en Markdown con selección de texto para navegadores Chromium.

> Chromium · Manifest V3 · SidePanel · Almacenamiento local

---

## ¿Por qué vkt-note?

La mayoría de extensiones de notas requieren cuentas, sincronización en la nube o suscripciones. vkt-note es diferente: **tus notas se quedan en tu navegador y nunca se suben.**

| Ventaja | Detalle |
|---------|--------|
| 📝 **Selección de texto** | Selecciona texto en cualquier página web, clic derecho para guardar como nota Markdown al instante |
| 🔒 **Solo local** | Todas las notas se almacenan en `chrome.storage.local` — sin nube, sin cuentas, sin rastreo |
| 🔐 **Cifrado real** | Protege una nota o todo el cuaderno con una contraseña — texto cifrado AES-256-GCM en reposo, claves nunca almacenadas |
| ✏️ **Editor Markdown** | Edición en código fuente con barra de herramientas de formato, guardado automático y vista previa Markdown en vivo |
| 🗑 **Papelera (Premium)** | Las eliminaciones Premium se pueden recuperar durante 30 días antes de borrarse automáticamente |

---

## Lista de funcionalidades

### 🆓 Funcionalidades gratuitas

| Funcionalidad | Descripción |
|---------|-------------|
| 📝 **Guardar en vkt-note** | Clic derecho en cualquier selección o imagen → el menú unificado detecta automáticamente el contenido, convierte HTML a Markdown y guarda silenciosamente — con el título de la página |
| 🔍 **Búsqueda de notas** | Filtra rápidamente la lista de notas por título y contenido |
| 📋 **Copiar como Markdown** | Un clic copia cualquier nota como Markdown al portapapeles — un respaldo local gratuito |
| ↩️ **Deshacer eliminación** | ¿Borraste una nota por error? Deshaz en 7 segundos desde la lista de notas |
| 📌 **Fijar arriba** | Mantén las notas frecuentes fijadas encima de la lista |
| 💾 **Descargar como .md** | Guarda cualquier nota como archivo Markdown — gratis, sin copiar y pegar |
| ✏️ **Editor Markdown** | Edición en código fuente con barra de herramientas de formato, guardado automático y vista previa Markdown en vivo |
| ☑️ **Listas de tareas** | Las listas `- [ ]` / `- [x]` se muestran como casillas reales en la vista previa |
| 🧩 **HTML → Markdown** | Usa la librería Turndown (estándar de la industria) para convertir HTML — tablas, encabezados, listas, enlaces, bloques de código, imágenes y más |
| ▦ **Selector de tablas** | Lista todas las tablas de la página actual — marca una o varias e insértalas en orden de página como Markdown; la página resalta las elegidas |
| 📏 **Insertar URL** | Inserta con un clic la URL de la página actual como enlace Markdown |
| 📑 **Insertar título** | Inserta con un clic el título de la página actual en la nota |
| 🛠️ **Barra de herramientas de formato** | Negrita, Cursiva, Tachado, H1–H3, Enlace, Código en línea, Bloque de código, Lista con viñetas/numerada, Cita, Regla horizontal |
| 💾 **Guardado automático** | Las notas se guardan automáticamente 2 segundos después de editar — no hace falta pulsar Guardar manualmente |
| ♾️ **Notas ilimitadas** | Sin límite diario: crea tantas notas como necesites |
| 🔢 **Contador de palabras** | La barra de estado muestra el total de notas y palabras (caracteres CJK y palabras latinas contados correctamente) |
| 🔐 **Contraseña por nota** | Bloquea una sola nota con su propia contraseña; tiene prioridad sobre la contraseña del cuaderno, así que solo se pide una contraseña |
| 🔒 **Contraseña del cuaderno** | Oculta todo el contenido de las notas tras una contraseña y mantiene los títulos en la lista; se desbloquea una vez por sesión del panel |
| 🔓 **Bloquear ahora** | Un clic elimina todas las claves de la memoria; cerrar el panel lateral también bloquea el cuaderno |
| 🔒 **Almacenamiento local** | Todas las notas se almacenan localmente — sin subida de notas, sin sincronización en la nube |
| 🏗️ **Manifest V3** | Construida sobre Manifest V3 con arquitectura SidePanel |

### ⭐ Funcionalidades Premium (requieren licencia)

| Funcionalidad | Descripción |
|---------|-------------|
| 📤 **Exportar todas las notas** | Descarga todas las notas como archivo JSON estructurado; las notas con contraseña permanecen cifradas |
| 🗑 **Papelera** | Las eliminaciones Premium van a la papelera, se pueden restaurar durante 30 días y después se eliminan automáticamente |

> Consulta [VKT Pricing](https://www.annmax1983.com/checkout.html?plugin=vktnote) para opciones de licencia.

---

## Vista previa

> 📸 Los recursos gráficos y las capturas de pantalla están en el directorio `screenshots/`.

---

## Navegadores compatibles

| Navegador | Estado | Versión mínima |
|---------|--------|-----------------|
| Google Chrome | ✅ Totalmente compatible | Chrome 116+ (sidePanel.open) |
| Microsoft Edge | ✅ Totalmente compatible | Edge 116+ |
| Otros navegadores basados en Chromium | ⚠️ Básico compatible | Debe soportar SidePanel API |

---

## Instalación

| Tienda | Enlace |
|---|---|
| Chrome Web Store | Próximamente 🚧 |
| Complementos de Microsoft Edge | [Instalar en Edge](https://microsoftedge.microsoft.com/addons/detail/imdfdonlhgecdhcfaapfohphcfnjgcef) |

> Instale solo desde las tiendas oficiales de arriba; evite sitios de descarga de terceros.

---

## Uso

### Crear notas

1. Haz clic en el **icono 📝 de vkt-note** en la barra de herramientas de tu navegador para abrir el panel lateral
2. Haz clic en **➕ Nueva nota** para crear una nota en blanco
3. O **selecciona texto** en cualquier página web → clic derecho → **Guardar en vkt-note**
4. O **clic derecho en una imagen** → **Guardar en vkt-note**

### Copiar contenido web como Markdown

- **Clic derecho en una selección** → **Guardar en vkt-note**. El HTML de la selección se convierte a Markdown usando la librería Turndown. Cuando la selección está dentro de una celda de tabla, se expande a la celda, fila o tabla completa (la unidad completa más pequeña).
- **Clic derecho en una imagen** → **Guardar en vkt-note**. El enlace de la imagen se guarda como imagen Markdown en una nueva nota.
- **▦ Selector de tablas** (barra de herramientas). Lista todas las tablas de la página actual; marca una o varias y pulsa **Insertar** — se convierten a Markdown y se añaden en orden de página (o en una nota nueva), y la página vuelve y resalta las tablas elegidas.

### Barra de herramientas de formato

La barra sobre el editor proporciona formato rápido: **Negrita**, *Cursiva*, ~~Tachado~~, H1, H2, H3, Enlace, Código en línea, Bloque de código, Lista con viñetas, Lista numerada, Cita, Regla horizontal.

### Editar notas

- Las notas **se guardan automáticamente 2 segundos** después de dejar de escribir — no hace falta pulsar Guardar manualmente
- El botón **Guardar** sigue funcionando para guardado inmediato
- Haz clic en **👁 Vista previa** para ver el Markdown renderizado en la pestaña de vista previa del editor
- Nota de vista previa: las listas anidadas profundamente se aplanan a un solo nivel en la vista previa (el Markdown guardado siempre mantiene la fidelidad completa)
- Las notas guardadas con clic derecho usan el título de la página de origen; las notas nuevas en blanco empiezan como `Note N` — ambas se pueden editar libremente

### Protección con contraseña

El cifrado es una función gratuita. Las contraseñas nunca se almacenan y tus notas se cifran en este dispositivo con AES-256-GCM antes de escribirse en `chrome.storage.local`.

- **Contraseña del cuaderno** — abre **Configuración → Contraseña del cuaderno** para establecer una. La lista de notas (títulos, fechas y recuentos de palabras) sigue visible; el contenido, los fragmentos y las coincidencias de búsqueda por contenido permanecen ocultos hasta que desbloquees. La contraseña se pide una vez por sesión del panel.
- **Contraseña por nota** — abre una nota, haz clic en el botón 🔐/🔒 de la cabecera del editor y elige **Establecer contraseña de nota**. Esa nota usará su propia contraseña. Una contraseña por nota **tiene prioridad** sobre la contraseña del cuaderno, así que nunca se te pedirán las dos.
- **Bloquear ahora** — el botón 🔒 de la cabecera del panel elimina de la memoria la clave del cuaderno y todas las claves de notas. Cerrar el panel lateral hace lo mismo. También puedes volver a pulsarlo para desbloquear.
- **Quitar una contraseña** — abre el diálogo de seguridad de la nota y elige **Quitar contraseña de la nota**, o quita la contraseña del cuaderno en Configuración. Quitar la contraseña del cuaderno descifra las notas protegidas y las devuelve a texto sin formato local; las contraseñas por nota se conservan.
- **Sin reglas de complejidad** — se acepta cualquier contraseña no vacía.
- **¿Olvidaste una contraseña?** — no hay recuperación. Eliminar la nota es la única forma de superar una contraseña por nota. Si olvidaste la contraseña del cuaderno, **Restablecer contraseña del cuaderno** elimina permanentemente todas las notas, elementos de la papelera y borradores protegidos por esa contraseña, y después desactiva la contraseña del cuaderno; las notas con su propia contraseña se conservan.

Las notas cifradas siguen siendo buscables por título, pero su contenido no se indexa ni se muestra en los fragmentos mientras están bloqueadas. La exportación JSON nunca descifra: las notas cifradas se exportan como texto cifrado y el diálogo de exportación te avisa primero. Como la extensión no importa notas, una exportación cifrada no sirve para leer esas notas: para conservar una copia legible, desbloquea la nota y usa **Copiar como Markdown** o **Descargar .md**. Mientras una contraseña del cuaderno está activa, un recorte pendiente del menú contextual se mantiene en `chrome.storage.session`, de modo que su texto sin formato no toca el disco.

### Papelera (Premium)

- Con Premium activo, eliminar una nota la mueve a la **Papelera** en lugar de borrarla.
- Los elementos de la papelera se pueden restaurar en cualquier momento dentro de **30 días**; después se eliminan automáticamente.
- **Vaciar papelera** y **Eliminar para siempre** eliminan los elementos de inmediato y no se pueden deshacer.
- Las eliminaciones del plan gratuito son permanentes: deshacer durante 7 segundos es la única recuperación.
- Si Premium caduca, los elementos existentes de la papelera siguen disponibles para restaurar o eliminar; solo las nuevas eliminaciones siguen la regla del plan gratuito.

### Notas sobre el nivel gratuito

- Sin límite diario de notas nuevas: el plan gratuito es un cuaderno completo, no una prueba
- Editar notas existentes es siempre ilimitado
- Los números de secuencia de títulos de notas pueden tener huecos después de eliminar — esto es intencionado

### Exportar y descargar

- **Nota individual → archivo .md**: pulsa el icono ⬇ en cualquier tarjeta de nota para descargarla como archivo Markdown (gratis)
- **Todas las notas → JSON** (Premium): pulsa **📥 Exportar** para descargar todas las notas en un archivo JSON estructurado; las notas con contraseña permanecen cifradas
- El archivo exportado es solo para respaldo/referencia — **la extensión no soporta importar notas**, por lo que las notas cifradas no se pueden leer ni restaurar desde ese archivo

---

## Preguntas frecuentes

1. **¿El menú de clic derecho no aparece?**
   El menú aparece cuando seleccionas texto o haces clic derecho en una imagen. Usa la opción unificada "Guardar en vkt-note".

2. **¿Las notas desaparecen al reinstalar?**
   Todas las notas se almacenan en `chrome.storage.local`. Desinstalar la extensión elimina permanentemente todos los datos. Exporta tus notas antes de desinstalar (Premium exporta todas las notas en un único archivo JSON, con las notas protegidas por contraseña en texto cifrado; el plan gratuito permite copiar o descargar las notas de una en una).

3. **¿Las imágenes en las notas se mueven rotas?**
   Las imágenes Markdown almacenan solo URLs remotas. Si el sitio web de origen no está disponible, bloquea el hotlinking o la imagen se elimina, la imagen no se cargará.

4. **¿Puedo importar las notas exportadas?**
   No. La exportación JSON es solo para respaldo manual. La extensión no soporta importar notas de vuelta.

5. **¿Hay un límite de notas nuevas?**
   No. Las notas nuevas son ilimitadas en ambos planes; Premium añade la exportación JSON completa y una papelera de 30 días.

6. **¿Olvidé mi contraseña? ¿Se puede recuperar?**
   No. La contraseña nunca se almacena, solo un verificador que no puede revertir el cifrado. Una contraseña por nota solo se puede eludir eliminando esa nota. Si olvidaste la contraseña del cuaderno, el proceso de restablecimiento elimina permanentemente todas las notas, elementos de la papelera y borradores protegidos por ella; las notas con contraseña propia sobreviven.

7. **¿Puedo ver los títulos de las notas cuando el cuaderno está bloqueado?**
   Sí. Los títulos, las fechas y los recuentos de palabras siguen visibles por diseño para que encuentres la nota que buscas; el contenido, los fragmentos y las coincidencias de búsqueda por contenido permanecen ocultos hasta que se desbloquee. La búsqueda por título sigue funcionando.

8. **¿Cómo se ven las notas cifradas en una exportación?**
   Se exportan como texto cifrado, no como texto sin formato. El diálogo de exportación te avisa cuando se incluyen notas cifradas. Como la extensión no importa notas, el archivo JSON no sirve para leer ni volver a importar esas notas. Para conservar una copia legible, desbloquea la nota y usa **Copiar como Markdown** o **Descargar .md**.

9. **¿Adónde van las notas eliminadas?**
   Con Premium, van a la Papelera y se pueden recuperar durante 30 días. En el plan gratuito, la eliminación es permanente después de los 7 segundos para deshacer.

---

## Privacidad

vkt-note sigue principios de privacidad desde el diseño:

- ✅ Todas las notas se almacenan en `chrome.storage.local` — **el contenido de las notas nunca se sube a ningún servidor**
- ✅ La protección con contraseña opcional cifra el contenido de las notas en reposo con AES-256-GCM (PBKDF2-HMAC-SHA256, 600.000 iteraciones); las contraseñas y las claves derivadas nunca se almacenan ni se transmiten
- ✅ La única solicitud saliente es la comprobación opcional de licencia Premium (clave de licencia, un identificador de instalación aleatorio, metadatos básicos del navegador) — sin notas, sin URL de páginas
- ✅ Sin analíticas, sin rastreo, sin cookies
- ✅ El contenido de la página se accede solo cuando activas explícitamente guardar o insertar (menú contextual, botones de insertar, selector de tablas) — nunca en segundo plano
- ✅ Los archivos JSON exportados se crean localmente y nunca se transmiten; las notas cifradas siguen siendo texto cifrado en las exportaciones

### Permisos

| Permiso | Razón |
|------------|--------|
| `storage` | Guardar notas y configuración localmente |
| `unlimitedStorage` | Eleva el límite de almacenamiento local predeterminado para que un historial de notas extenso nunca provoque un fallo de escritura |
| `sidePanel` | Mostrar la interfaz de la extensión en un panel lateral |
| `contextMenus` | Menú de clic derecho para crear notas desde texto seleccionado o imágenes |
| `scripting` | Inyectar el conversor HTML→Markdown solo cuando activas guardar / insertar / acciones de tabla |
| `alarms` | Ejecutar la tarea diaria que elimina los elementos de la papelera con más de 30 días |
| Host `<all_urls>` | Permite que esas acciones explícitas lean la selección, tablas, URL y título de la página actual — sin acceso en segundo plano ni al historial de navegación |

- [Política de privacidad completa](https://annmax1983.github.io/vkt-note/privacy-policy.html)

---

## Aviso de derechos de autor

1. Esta extensión permite a los usuarios guardar selecciones de texto y enlaces de imágenes de páginas web en notas locales. Todo el texto, las imágenes y los derechos de autor del contenido de cada sitio web pertenecen a su respectivo editor.
2. Guardar extractos como notas no otorga a los usuarios ninguna autorización de derechos de autor sobre el contenido del sitio web. Queda estrictamente prohibido usar esta extensión para eludir muros de pago, restricciones de membresía o mecanismos de protección contra copia de los sitios web.
3. Los usuarios deberán cumplir con las leyes locales y los términos de servicio de las plataformas al usar esta extensión.

---

## Aviso sobre el código fuente

> ⚠️ **Este repositorio se mantiene para el desarrollo y el empaquetado de versiones.** El código fuente es propietario y no puede redistribuirse ni reempaquetarse. La extensión se distribuye a través de las tiendas oficiales de extensiones del navegador (Chrome Web Store y Microsoft Edge Add-ons); no se proporcionan paquetes de instalación sin conexión.

---

## Licencia

Copyright © 2026 vkt-note. Todos los derechos reservados.

Este software es de código cerrado y propietario. Sin autorización escrita oficial, quedan estrictamente prohibidos:
- Descompilar, piratear o modificar el código del programa
- Reempaquetar, redistribuir, compartir o reventa comercial
- Incorporar el programa a otro software para distribución conjunta

---

## ❤️ Apoyo

Si te resulta útil vkt-note, ¡considera invitar al desarrollador a un café!

**[👉 Haz clic aquí para apoyar](https://ko-fi.com/annmax?buyACoffee=true&ref=vkt-note)**
