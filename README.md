# taller-integrador-castro cortyes 1 y 2
**Asignatura:** Buenas Prácticas de Desarrollo de Software
**Estudiante:** José Miguel Castro Mercado
**Institución:** Corporación Universidad de la Costa (CUC)

📋 Auditoría del Sitio Web (Tabla de Hallazgos)

| Defecto encontrado | Por qué era un problema | Cómo lo corrigió |
| :--- | :--- | :--- |
| Nombres de archivos con espacios y mayúsculas | Ocasiona incompatibilidades en servidores Linux, URLs inestables y problemas de ruta en Git. | Se renombraron los archivos a minúsculas y sin espacios (`index.html` y `styles.css`). |
| Título genérico en la pestaña browser | No brinda contexto ni accesibilidad adecuada al usuario. | Se configuró un título semántico: `<title>Calculadora de Notas</title>`. |
| Identificadores HTML no semánticos (`id="n1"`, `id="btn"`) | Dificulta la lectura del DOM y el mantenimiento del código JS/CSS. | Se renombraron usando camelCase descriptivo (`id="nota1"`, `id="btnCalcular"`, `id="resultado"`). |
| Variables JS poco descriptivas (`var x`, `var y`) | No comunican la intención del dato y obligan a revisar todo el contexto para entenderlas. | Se declararon variables descriptivas (`const nota1`, `let promedio`) en JS. |
| Uso de `var` y función con nombre impreciso | `var` genera scope global ambiguo y hoisting; el nombre no indica claramente la función. | Se reemplazó por `const`/`let` y se nombró la función `calcularPromedio()`. |
| Líneas de código sobrantes y `console.log` | Generan código basura (*dead code*) y ensucian la consola en producción. | Se removieron todas las instrucciones e improntas sin utilidad práctica. |
| Mala indentación y formato desordenado | Dificulta la lectura rápida del código entre distintos desarrolladores del equipo. | Se formateó el código HTML y CSS siguiendo estándares de identación limpia. |
| Enlace de hoja de estilos roto tras renombrado | El archivo HTML no carga los estilos CSS si la ruta no coincide exactamente. | Se corrigió la etiqueta `<link rel="stylesheet" href="styles.css">` en el `<head>`. |

## 🌐 Enlaces del Proyecto
* **Sitio Web Publicado (Netlify):** `[INSERTAR_TU_LINK_DE_NETLIFY]`
* **Repositorio en GitHub:** `https://github.com/josemcastrom91/taller-integrador-castro`
