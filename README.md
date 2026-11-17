# Portafolio profesional · Luis Eduardo Mendoza Roman

**Identidad de autor:** MRL / Leonhardt  
**GitHub:** https://github.com/Mr-LuisEd  
**LinkedIn:** https://www.linkedin.com/in/luis-mendoza-293538273/

Este proyecto está preparado para **GitHub Pages** y no necesita PHP ni servidor propio. Funciona con HTML, CSS, JavaScript y datos en `data.json`.

## Qué contiene

- `index.html`: sitio público, diseño adaptable, selector **ES/EN**, proyectos con imágenes, estudios, certificaciones, experiencia y contacto.
- `admin.html`: pestaña **Mi cuenta** para editar textos, formación, certificados, experiencia y proyectos.
- `data.json`: todos los datos editables; contiene los campos españoles y opcionales terminados en `_en` para la versión inglesa.
- `imagenes/kit_leonhardt.png`: captura real de la interfaz del Kit de Soporte Leonhardt, proporcionada por el autor.
- `imagenes/kit_archivos.png`: segunda captura del kit (explorador de archivos).
- `imagenes/portafolio_web.png`: vista de una versión anterior del portafolio (referencia visual).
- `imagenes/app_habitos_portada.webp`: detalle de la pantalla principal para la tarjeta de proyecto.
- `imagenes/app_habitos_inicio.webp`: captura de la página principal, con metas y hábitos.
- `imagenes/app_habitos_detalle.webp`: captura con rachas, historial y calendario.
- `imagenes/app_habitos_resumen.webp`: captura con hábitos y resumen semanal.
- `imagenes/portada-compartir.jpg`: portada social de enlace en LinkedIn y redes.
- `foto.jpg`: fotografía de presentación.
- `certificados/`: once PDFs individuales Oracle/Cisco y constancia de la Hackatón Transformagob 2026.
- `CV_Luis_Eduardo_Mendoza_Roman_Publico.pdf`: CV público de una página sin DNI ni dirección particular.

El proyecto **App de hábitos y objetivos** aparece como *prototipo en desarrollo*, ahora con cuatro imágenes basadas en capturas reales del 17/11/2026: portada, pantalla principal, detalle de un hábito y resumen semanal. Las capturas permiten documentar las pantallas, pero aún no se ha inspeccionado su código fuente ni comprobado en dispositivo todas las interacciones. La pila Kotlin/Jetpack Compose refleja el plan del proyecto y debe verificarse antes de presentarla como implementación final.

## Publicar en GitHub Pages

1. **Revisa la información pública antes de subir los archivos.** Los certificados contienen tu nombre completo y fechas. No incluyas documentos con DNI, direcciones privadas, contraseñas ni conversaciones de terceros.
2. Entra a tu repositorio `https://github.com/Mr-LuisEd/mi-primer-portafolio`.
3. Haz una copia de seguridad de los archivos del repositorio actual.
4. **Descomprime este ZIP** en tu computadora. Sube **los archivos y carpetas de su interior** a la raíz de la rama `main`, no el ZIP completo.
5. En GitHub: `Settings → Pages → Build and deployment → Deploy from a branch → main / (root) → Save`.
6. Cuando GitHub Pages indique que el sitio está publicado, revisa la dirección que muestre (normalmente `https://mr-luised.github.io/mi-primer-portafolio/`). Verifica que carguen `data.json`, fotografías, enlaces y PDFs.
7. Comprueba los botones **ES/EN**, los enlaces de certificados, los proyectos en móvil y la descarga del CV.

> GitHub Pages es estático; **PHP no se ejecuta** allí. En caso de cambiar de plataforma o dominio, actualiza las etiquetas `og:image`, `og:url` y `canonical` del `<head>` de `index.html`.

## Cómo funciona «Mi cuenta»

1. Abre el sitio publicado por **HTTPS** y elige **Mi cuenta**.
2. Para editar el repositorio, crea un **GitHub fine-grained personal access token** desde `https://github.com/settings/personal-access-tokens/new`:
   - Resource owner: `Mr-LuisEd`.
   - Repository access: **Only select repositories** → `mi-primer-portafolio`.
   - Repository permissions → **Contents: Read and write**.
   - Vencimiento corto; no des permisos adicionales.
3. Introduce el token **solo en el formulario de la web oficial que acabas de publicar**. No lo compartas por chat ni lo incluyas en archivos ni capturas. El panel lo mantiene en memoria durante la sesión, **no en almacenamiento local**.
4. Actualiza los elementos en sus pestañas y usa **Guardar en borrador** o **Guardar borrador local**. Los borradores locales contienen solo los textos y rutas, nunca el token.
5. Pulsa **Vista previa ES / EN**. Se abrirá otra pestaña con una banda que indica que no está publicada. Puedes revisar ambas versiones allí.
6. Cuando todo esté correcto, elige **Publicar cambios**. Se actualizará `data.json` con un commit en GitHub.
7. Pulsa **Cerrar sesión**. Se recomienda revocar el token cuando ya no se vaya a utilizar.

### Opciones disponibles

- **Presentación:** titulares, biografía y disponibilidad en español e inglés.
- **Estudios:** agrega SENATI, UTP o futuros grados académicos solo cuando se cumplan realmente.
- **Certificados:** agregar, modificar, reordenar, eliminar y subir PDFs individuales de hasta 4 MB.
- **Experiencia:** actualizar puestos, instituciones, periodos y responsabilidades.
- **Proyectos:** añadir nombres, descripción ES/EN, tecnologías, estado, repositorio, imagen principal y galería por rutas. También se pueden subir imágenes PNG/JPG/WEBP de hasta 4 MB.
- **Archivos:** reemplazar fotografía JPG y CV público PDF de hasta 4 MB.
- **Vista de muestra:** permite practicar con el editor sin autenticar ni publicar.

**Limitaciones:** Los archivos que subes desde «Mi cuenta» se publican directamente en el repositorio antes de que publiques el registro de `data.json`. Si cierras sin publicar, podría quedar un archivo sin enlace. El CV no cambia automáticamente al editar `data.json`: reemplázalo también cuando actualices tu formación. El panel no es una aplicación con cuentas internas y contraseñas: su escritura depende del permiso temporal de GitHub. No se probó un inicio de sesión real con token, porque el token es privado y solo tú debes usarlo.

## Cambios de esta versión

- Marca de autor **MRL · Leonhardt**, manteniendo el nombre completo como perfil profesional.
- Imagen real del Kit de Soporte Leonhardt y captura secundaria.
- App de hábitos descrita como prototipo en desarrollo, con tres capturas reales completas y una portada recortada, sin exagerar funciones aún no verificadas.
- Habilidades separadas en **utilizadas** y **en aprendizaje**.
- Interfaz ES/EN y textos bilingües editables desde «Mi cuenta».
- Borrador local, previsualización previa a publicar y confirmación antes de eliminar.
- Certificados como PDFs individuales, con botones para consultarlos, sin publicar el documento combinado original.
- Portada para vista previa en redes sociales.
- CV público actualizado, sin información privada innecesaria.

## Prueba local

**Ahora sí puedes abrir `index.html` haciendo doble clic:** la página incluye una copia inicial de `data.json` y mostrará tus 11 certificados y 3 proyectos sin necesitar un servidor. Cuando se publique por HTTPS, usará el `data.json` del repositorio para reflejar las actualizaciones hechas desde **Mi cuenta**. Si editas `data.json` localmente sin servir HTTP, la vista offline seguirá mostrando el respaldo integrado de esta entrega.

Si tienes Python instalado, desde la carpeta descomprimida ejecuta:

```bash
python -m http.server 8000
```

Luego abre `http://localhost:8000/` en tu navegador para probar el portafolio y el **modo de muestra** del editor. Para publicar los cambios desde «Mi cuenta» debes utilizar la versión HTTPS de GitHub Pages.

**Estado:** proyecto empaquetado y comprobado a nivel de sintaxis, archivos y enlaces locales. Falta probar en tu propio navegador el inicio de sesión con GitHub y las operaciones de publicación del repositorio; no se ha actualizado tu GitHub automáticamente.

## Código abierto y permanencia

- El repositorio será **público**. GitHub Pages permite servir una web estática mientras el repositorio, la cuenta y el servicio sigan activos y se respeten las políticas de GitHub; no hay garantía de permanencia indefinida.
- «Repositorio público» **no equivale automáticamente a licencia de código abierto**. Por defecto, los derechos sobre código, fotografías y certificados siguen reservados. Para permitir reutilización del código, agrega una licencia apropiada (por ejemplo MIT), excluyendo fotografías, certificados y documentos personales.
- No subas ejecutables de software propietario, activadores ni contraseñas dentro del portafolio público.

## Licencia del código

El código fuente del portafolio está disponible bajo licencia [MIT](LICENSE). Esto permite reutilización y adaptación del código siempre que se conserve el aviso de copyright. **No están licenciados bajo MIT** los archivos de `certificados/`, `foto.jpg`, el CV, las imágenes del portafolio ni los logotipos de terceros. El acceso público a esos materiales no otorga permiso para reutilizarlos.

**Publicación segura:** los archivos subidos a un repositorio público se pueden descargar y conservar por terceros. Revisa su contenido antes de publicarlos.

## Archivos de certificados actualizados el 17/11/2026

Se incorporaron los **11 PDF individuales originales** recibidos del autor (diez Cisco Networking Academy y uno de Oracle Academy), manteniendo la constancia de Hackatón de una entrega previa.

- El PDF escaneado **Pagapu Wanka 2024** no se muestra en la galería técnica por tratarse de una participación cultural; se puede añadir posteriormente a una sección de voluntariado o participación comunitaria.
- El certificado escaneado de **Java Foundations** contiene un apellido que debe verificarse con Oracle Academy si difiere del nombre legal; el portafolio lo describe como constancia de finalización de curso, no como certificación profesional oficial por examen.
- Los archivos PDF originales son propiedad de sus emisores; su publicación permite consulta, no reutilización bajo la licencia MIT del código.

## Solución del problema «Cargando certificados…»

La versión anterior solo mostraba un proyecto y se quedaba en «Cargando certificados…» si abrías `index.html` directamente desde Descargas. La versión actual incorpora una copia de lectura en el HTML que se visualiza desde `file://`, mientras que en GitHub Pages sigue actualizando el contenido desde `data.json`.

Nota de presentación: se giró únicamente la orientación de visualización del PDF escaneado de Oracle para que se lea horizontalmente; el contenido del certificado no se alteró.
