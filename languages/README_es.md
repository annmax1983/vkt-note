# vkt-note

[English](../README.md) | [中文](README_zh.md) | [Deutsch](README_de.md) | Español | [日本語](README_ja.md) | [Français](README_fr.md)

Manual de usuario oficial · Una extensión ligera de notas en Markdown con selección de texto para navegadores Chromium.

> Chromium · Manifest V3 · SidePanel · Almacenamiento local

---

## ¿Por qué vkt-note?

La mayoría de extensiones de notas requieren cuentas, sincronización en la nube o suscripciones. vkt-note es diferente: **todo se queda en tu navegador, cero datos salen de tu dispositivo.**

| Ventaja | Detalle |
|---------|--------|
| 📝 **Selección de texto** | Selecciona texto en cualquier página web, clic derecho para guardar como nota Markdown al instante |
| 🔒 **Solo local** | Todas las notas se almacenan en `chrome.storage.local` — sin nube, sin cuentas, sin rastreo |
| ✏️ **Editor Markdown** | Edición en código fuente con barra de herramientas de formato, guardado automático y vista previa a pantalla completa |
| 📎 **Seguimiento de origen** | Enlace a la página de origen visible en la barra de pestañas del editor — siempre sabrás de dónde vienen tus notas |
| 📋 **Cuota inteligente** | 3 notas/día gratis; elimina las notas de hoy para recuperar espacios — nunca te quedarás bloqueado |

---

## Lista de funcionalidades

### 🆓 Funcionalidades gratuitas

| Funcionalidad | Descripción |
|---------|-------------|
| 📝 **Guardar en vkt-note** | Clic derecho en cualquier selección o imagen → el menú unificado detecta automáticamente el contenido, convierte HTML a Markdown y guarda silenciosamente |
| 🔍 **Búsqueda de notas** | Filtra rápidamente la lista de notas por título y contenido |
| 📋 **Copiar como Markdown** | Un clic copia cualquier nota como Markdown al portapapeles — un respaldo local gratuito |
| ✏️ **Editor Markdown** | Edición en código fuente con barra de herramientas de formato, guardado automático y vista previa a pantalla completa |
| 🧩 **HTML → Markdown** | Usa la librería Turndown (estándar de la industria) para convertir HTML — tablas, encabezados, listas, enlaces, bloques de código, imágenes y más |
| ▦ **Selector de tablas** | Lista todas las tablas de la página actual — elige una para insertarla como tabla Markdown |
| 📏 **Insertar URL** | Inserta con un clic la URL de la página actual como enlace Markdown |
| 📑 **Insertar título** | Inserta con un clic el título de la página actual en la nota |
| 🔗 **Enlace a página de origen** | Enlace clicable al origen visible en la barra de pestañas del editor para notas creadas desde páginas web |
| 🛠️ **Barra de herramientas de formato** | Negrita, Cursiva, Tachado, H1–H3, Enlace, Código en línea, Bloque de código, Lista con viñetas/numerada, Cita, Regla horizontal |
| 💾 **Guardado automático** | Las notas se guardan automáticamente 2 segundos después de editar — no hace falta pulsar Guardar manualmente |
| 📋 **Cuota diaria** | 3 notas nuevas por día; editar notas existentes no consume cuota |
| 🔒 **Almacenamiento local** | Todas las notas se almacenan localmente — sin subida de datos, sin sincronización en la nube |
| 🏗️ **Manifest V3** | Construida sobre Manifest V3 con arquitectura SidePanel |

### ⭐ Funcionalidades Premium (requieren licencia)

| Funcionalidad | Descripción |
|---------|-------------|
| ♾️ **Notas ilimitadas** | Sin cuota diaria — crea tantas notas como quieras |
| 📤 **Exportar todas las notas** | Descarga todas las notas como archivo de respaldo JSON estructurado |
| 💬 **Soporte prioritario** | Soporte prioritario por correo electrónico para usuarios Premium |

> Consulta [VKT Pricing](https://www.annmax1983.com/pricing.html) para opciones de licencia.

---

## Vista previa

> 📸 Las capturas de pantalla se publicarán aquí con el listado de la tienda.

---

## Navegadores compatibles

| Navegador | Estado | Versión mínima |
|---------|--------|-----------------|
| Google Chrome | ✅ Totalmente compatible | Chrome 114+ (SidePanel API) |
| Microsoft Edge | ✅ Totalmente compatible | Edge 114+ |
| Otros navegadores basados en Chromium | ⚠️ Básico compatible | Debe soportar SidePanel API |

---

## Instalación

Por tu seguridad, instala vkt-note solo a través de las tiendas oficiales de extensiones del navegador:

1. Abre **Chrome Web Store** o **Microsoft Edge Add-ons**
2. Busca: `vkt-note`
3. Haz clic en **"Añadir a Chrome"** / **"Añadir a Edge"**
4. Haz clic en el icono 📝 de vkt-note en tu barra de herramientas para abrir el panel lateral

> ⚠️ No instales desde sitios web de terceros. Las versiones no autorizadas pueden comprometer la seguridad de tus datos.

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
- **▦ Selector de tablas** (barra de herramientas). Lista todas las tablas de la página actual; haz clic en una para insertarla como tabla Markdown en la nota abierta (o en una nueva nota).

### Barra de herramientas de formato

La barra sobre el editor proporciona formato rápido: **Negrita**, *Cursiva*, ~~Tachado~~, H1, H2, H3, Enlace, Código en línea, Bloque de código, Lista con viñetas, Lista numerada, Cita, Regla horizontal.

### Editar notas

- Las notas **se guardan automáticamente 2 segundos** después de dejar de escribir — no hace falta pulsar Guardar manualmente
- El botón **Guardar** sigue funcionando para guardado inmediato
- Haz clic en **👁 Vista previa** para ver el contenido formateado en una **vista a pantalla completa** con un botón de volver — sin el editor visible
- Nota de vista previa: las listas anidadas profundamente se aplanan a un solo nivel en la vista previa (el Markdown guardado siempre mantiene la fidelidad completa)
- **Enlace a página de origen**: al editar una nota creada desde una página web, se muestra un enlace clicable al origen en la barra de pestañas del editor
- Los títulos se generan automáticamente como `笔记YYYYMMDD_N` — puedes editarlos libremente

### Reglas del nivel gratuito

- Versión gratuita: máximo **3 notas nuevas por día**
- Solo pulsar **Guardar** en una **nota nueva** cuenta para el límite diario
- Editar notas existentes **no** consume cuota
- Eliminar una nota creada **hoy** restaura un espacio de cuota
- Eliminar una nota de un día anterior **no** afecta a la cuota de hoy
- Los números de secuencia de títulos de notas pueden tener huecos después de eliminar — esto es intencionado

### Exportar (Solo Premium)

- Los usuarios Premium pueden hacer clic en **📥 Exportar** para descargar todas las notas como archivo JSON
- El archivo exportado es solo para respaldo/referencia — **la extensión no soporta importar notas**

---

## Preguntas frecuentes

1. **¿El menú de clic derecho no aparece?**
   El menú aparece cuando seleccionas texto o haces clic derecho en una imagen. Usa la opción unificada "Guardar en vkt-note".

2. **¿Las notas desaparecen al reinstalar?**
   Todas las notas se almacenan en `chrome.storage.local`. Desinstalar la extensión elimina permanentemente todos los datos. Exporta tus notas antes de desinstalar (funcionalidad Premium).

3. **¿Las imágenes en las notas se mueven rotas?**
   Las imágenes Markdown almacenan solo URLs remotas. Si el sitio web de origen no está disponible, bloquea el hotlinking o la imagen se elimina, la imagen no se cargará.

4. **¿Puedo importar las notas exportadas?**
   No. La exportación JSON es solo para respaldo manual. La extensión no soporta importar notas de vuelta.

5. **¿Cómo consigo más de 3 notas por día?**
   Elimina las notas creadas hoy para liberar espacios, o actualiza a Premium para notas ilimitadas.

---

## Privacidad

vkt-note sigue principios de privacidad desde el diseño:

- ✅ Todas las notas se almacenan en `chrome.storage.local` — **no se suben datos a ningún servidor**
- ✅ Sin analíticas, sin rastreo, sin cookies
- ✅ El contenido de la página se accede solo cuando activas explícitamente guardar o insertar (menú contextual, botones de insertar, selector de tablas) — nunca en segundo plano
- ✅ Los archivos JSON exportados se crean localmente y nunca se transmiten

### Permisos

| Permiso | Razón |
|------------|--------|
| `storage` | Guardar notas y configuración localmente |
| `sidePanel` | Mostrar la interfaz de la extensión en un panel lateral |
| `contextMenus` | Menú de clic derecho para crear notas desde texto seleccionado o imágenes |
| `scripting` | Inyectar el conversor HTML→Markdown solo cuando activas guardar / insertar / acciones de tabla |
| Host `<all_urls>` | Permite que esas acciones explícitas lean la selección, tablas, URL y título de la página actual — sin acceso en segundo plano ni al historial de navegación |

- [Política de privacidad completa](https://annmax1983.github.io/vkt-note/privacy-policy.html)

---

## Aviso de derechos de autor

1. Esta extensión permite a los usuarios guardar selecciones de texto y enlaces de imágenes de páginas web en notas locales. Todo el texto, las imágenes y los derechos de autor del contenido de cada sitio web pertenecen a su respectivo editor.
2. Guardar extractos como notas no otorga a los usuarios ninguna autorización de derechos de autor sobre el contenido del sitio web. Queda estrictamente prohibido usar esta extensión para eludir muros de pago, restricciones de membresía o mecanismos de protección contra copia de los sitios web.
3. Los usuarios deberán cumplir con las leyes locales y los términos de servicio de las plataformas al usar esta extensión.

---

## Aviso sobre el código fuente

> ⚠️ **Este repositorio no publica código fuente.** Contiene únicamente documentación de uso, notas de lanzamiento y recursos de soporte. La extensión se distribuye exclusivamente a través de Chrome Web Store. No se proporcionan paquetes de instalación sin conexión ni código fuente para usuarios finales.

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
