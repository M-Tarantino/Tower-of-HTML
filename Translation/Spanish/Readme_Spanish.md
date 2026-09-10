#Tower of HTML

> **Haz que la educación sobre HTML sea universalmente accesible, sin importar el hardware, la conectividad a internet o la antigüedad del dispositivo.**

**Tower of HTML** es una plataforma educativa minimalista y centrada en el funcionamiento sin conexión (*offline-first*) diseñada para enseñar los fundamentos de HTML desde cero. Toda la aplicación se encuentra dentro de un único archivo `.html` autónomo sin dependencias externas, frameworks, pasos de compilación o requisitos de servidor.

---

## 📋 Tabla de contenidos

- [Filosofía de diseño y misión principal](#filosofía-de-diseño-y-misión-principal)
- [Características principales](#características-principales)
- [Accesibilidad universal y compatibilidad de hardware](#accesibilidad-universal-y-compatibilidad-de-hardware)
- [Primeros pasos](#primeros-pasos)
- [Arquitectura y mecánica](#arquitectura-y-mecánica)
- [Ruta de aprendizaje (51 pisos)](#ruta-de-aprendizaje-51-pisos)
- [Sistema de progresión por códigos de nivel](#sistema-de-progresión-por-códigos-de-nivel)
- [Pautas de personalización y extensión](#pautas-de-personalización-y-extensión)
- [Progreso de traducción de idiomas](#progreso-de-traducción-de-idiomas)
- [Especificaciones técnicas](#especificaciones-técnicas)
- [Licencia y autor](#licencia-y-autor)

---

## 🎯 Filosofía de diseño y misión principal

### El problema que resolvemos
La mayoría de las plataformas modernas de aprendizaje de desarrollo web presentan barreras importantes:
1. **Dependencia de la conectividad a internet**: Los IDE en línea y las plataformas LMS fallan en entornos de bajo ancho de banda o sin conexión.
2. **Requisitos de hardware moderno**: Las herramientas modernas requieren sistemas operativos modernos, alta memoria RAM y motores de navegador pesados, lo que excluye a los usuarios con hardware antiguo.
3. **Sobrecarga de complejidad**: Los principiantes suelen abrumarse con herramientas de compilación, frameworks y administradores de paquetes antes de escribir una sola línea de HTML.
4. **Bloqueo de proveedor (Vendor Lock-in)**: El progreso del usuario depende de la disponibilidad de la plataforma de terceros y de la creación obligatoria de cuentas.

### Nuestra solución
Tower of HTML opera sobre cuatro compromisos fundamentales:
* **Accesibilidad antes que características**: Prioriza la compatibilidad pura y la legibilidad clara por encima de los frameworks de interfaz de usuario.
* **Educación por encima del entretenimiento**: Progresión estructurada piso por piso donde el dominio se gana mediante una validación estricta y justa.
* **Propiedad por encima de las plataformas**: Los usuarios pueden poseer, descargar, modificar y ejecutar el proyecto indefinidamente sin pedir permiso.
* **Claridad por encima de la astucia**: Escrito en código claro y legible sin ofuscación ni transpilación para que los estudiantes puedan inspeccionar y aprender directamente del código fuente.

---

## ✨ Características principales

* **100% Offline-First**: Se ejecuta localmente en cualquier navegador web sin requerir acceso a la red.
* **Arquitectura de archivo único**: Todo (CSS, JS, Contenido) reside dentro de un único archivo `index.html` portátil (~50 KB).
* **Soporte para motores antiguos**: Construido utilizando JavaScript seguro para sistemas heredados (estándar ES3/ES5) para garantizar una ejecución funcional en hardware antiguo.
* **Cero dependencias**: Libre de bibliotecas externas, administradores de paquetes, fuentes o enlaces CDN.
* **Sistema de códigos de nivel**: Un mecanismo simple de hash de contraseñas permite a los usuarios reanudar el progreso en cualquier navegador o dispositivo sin almacenamiento local.
* **Temas de terminal**: Modos visuales personalizables (Matrix, Amber, DOS Blue, Light, Cyber) accesibles directamente en la interfaz.

---

## 🌐 Accesibilidad universal y compatibilidad de hardware

Debido a que Tower of HTML está escrito en JavaScript seguro para sistemas heredados sin dependencias web modernas, se ejecuta de manera confiable en un amplio espectro de dispositivos y sistemas operativos:

| Dispositivo / Plataforma | Estado operativo | Notas |
| :--- | :---: | :--- |
| **PC Pentium de 1995** | ✅ Compatible | Windows 95/98, Internet Explorer 6+ |
| **Chromebooks** | ✅ Compatible | Todas las versiones del navegador Chrome |
| **Móviles antiguos (iPhone 4S / Android 4.0)** | ✅ Compatible | Navegadores móviles nativos (Safari 5+, Android WebKit) |
| **Laptops y escritorios modernos** | ✅ Compatible | Chrome, Firefox, Safari, Edge, Opera |
| **Raspberry Pi** | ✅ Compatible | Motores de navegador ligeros |
| **Laboratorios educativos de bajos recursos** | ✅ Compatible | Sin privilegios administrativos ni instalación requerida |

Este diseño permite a los educadores en entornos de bajos recursos descargar el proyecto una vez y distribuirlo a los estudiantes a través de USB o compartir archivos locales.

---

## 🚀 Primeros pasos

1. Descarga o guarda el archivo `index.html` en tu dispositivo.
2. Haz doble clic en `index.html` (o ábrelo con cualquier navegador web).
3. Lee las indicaciones para el piso actual, escribe tu fragmento de HTML en el campo de entrada y haz clic en **CHECK CODE** (Comprobar código).
4. Al completar un piso, anota o copia el **Código de nivel (Level Code)** generado para reanudar tu progreso en sesiones futuras o en diferentes dispositivos.

---

## 🏗️ Arquitectura y mecánica

El archivo único `index.html` separa estrictamente la lógica de ejecución del contenido educativo manteniendo un entorno libre de dependencias:


index.html
├── <head>
│   └── <style> : Estilos de terminal, diseños adaptativos, temas visuales
└── <body>
├── Contenedor UI : Pantalla de juego, terminal de entrada, vista de salida
└── <script>
├── Matriz levels[] : Datos instructivos de texto plano y reglas de validación
└── Lógica del motor : Actualizaciones del DOM, verificación de códigos de nivel, estado de progresión

### Compromisos de diseño
- **CSS en línea**: Incrustado dentro de un único bloque `<style>`.
- **JavaScript en línea**: Incrustado dentro de un único bloque `<script>`.
- **Estándar ES3/ES5**: Utiliza construcciones de bucles estándar y sintaxis ES3/ES5 (`var`, bucles `for`) en lugar de características modernas de ES6+ que requieren transpilación.

---

## 📚 Ruta de aprendizaje (51 pisos)

El plan de estudios consta de 51 pisos estructurados que abarcan seis fases distintas:


Progresión de habilidades:
Principiante (Pisos 0–8)    → Etiquetas, etiquetas de cierre y estructura de página
Intermedio (Pisos 9–28)    → Formato, enlaces, botones y multimedia
Avanzado (Pisos 29–48)     → Divisiones, listas, formularios, tablas y atributos
Experto (Pisos 49–51)      → Declaraciones de documentos, conjuntos de caracteres e integración final

### Fase 1: Fundamentos (Pisos 0–8)
| Piso | Código | Título | Tarea / Concepto |
| :---: | :--- | :--- | :--- |
| **0** | `START` | Descripción general e instrucciones | Introducción al juego y controles |
| **1** | `L1-ROOT` | El elemento raíz | Creación de la etiqueta `<html>` |
| **2** | `L2-HEAD` | La sección de cabecera | Contenedor de metadatos `<head>` |
| **3** | `L3-TITLE` | Título de la página | Nomenclatura de pestaña `<title>` |
| **4** | `L4-BODY` | La sección del cuerpo | Área de contenido `<body>` |
| **5** | `L5-PARA` | Párrafos | Estructura de texto `<p>` |
| **6** | `L6-CLOSE-P` | Cierre de etiqueta de párrafo | Cierre de etiqueta `</p>` |
| **7** | `L7-CLOSE-BODY` | Cierre de etiqueta de cuerpo | Cierre de etiqueta `</body>` |
| **8** | `L8-CLOSE-HTML` | Cierre de etiqueta HTML | Cierre de etiqueta `</html>` |

### Fase 2: Contenido y texto (Pisos 9–18)
| Piso | Código | Título | Tarea / Concepto |
| :---: | :--- | :--- | :--- |
| **9** | `L9-H1` | Encabezado principal (H1) | Nivel de encabezado 1 `<h1>` |
| **10** | `L10-H2` | Subencabezado (H2) | Nivel de encabezado 2 `<h2>` |
| **11** | `L11-CLOSE-H1` | Cerrar etiqueta de encabezado | Etiqueta de cierre `</h1>` |
| **12** | `L12-BOLD` | Texto en negrita | Negrita de presentación `<b>` |
| **13** | `L13-CLOSE-BOLD` | Cerrar etiqueta de negrita | Cierre de etiqueta `</b>` |
| **14** | `L14-ITALIC` | Texto en cursiva | Cursiva de presentación `<i>` |
| **15** | `L15-CLOSE-ITALIC` | Cerrar etiqueta de cursiva | Cierre de etiqueta `</i>` |
| **16** | `L16-STRONG` | Énfasis fuerte | Énfasis semánticamente importante `<strong>` |
| **17** | `L17-CLOSE-STRONG` | Cerrar etiqueta de énfasis fuerte | Cierre de etiqueta `</strong>` |
| **18** | `L18-EM` | Énfasis | Énfasis semántico `<em>` |

### Fase 3: Enlaces y multimedia (Pisos 19–28)
| Piso | Código | Título | Tarea / Concepto |
| :---: | :--- | :--- | :--- |
| **19** | `L19-ANCHOR` | Etiqueta de enlace | Elemento de anclaje `<a>` |
| **20** | `L20-HREF` | Destino del enlace | Uso del atributo `<a href="...">` |
| **21** | `L21-CLOSE-ANCHOR` | Cerrar etiqueta de enlace | Cierre de etiqueta `</a>` |
| **22** | `L22-IMG` | Elemento de imagen | Contenedor de imagen `<img>` |
| **23** | `L23-SRC` | Fuente de la imagen | Uso del atributo `<img src="...">` |
| **24** | `L24-ALT` | Texto alternativo | Atributo de accesibilidad (`alt="..."`) |
| **25** | `L25-BR` | Salto de línea | Salto de línea autocerrado `<br>` |
| **26** | `L26-HR` | Línea horizontal | Línea divisoria `<hr>` |
| **27** | `L27-BUTTON` | Elemento de botón | Elemento interactivo `<button>` |
| **28** | `L28-CLOSE-BUTTON` | Cerrar etiqueta de botón | Cierre de etiqueta `</button>` |

### Fase 4: Organización (Pisos 29–38)
| Piso | Código | Título | Tarea / Concepto |
| :---: | :--- | :--- | :--- |
| **29** | `L29-DIV` | Contenedor de división | Contenedor en bloque `<div>` |
| **30** | `L30-CLOSE-DIV` | Cerrar etiqueta DIV | Cierre de etiqueta `</div>` |
| **31** | `L31-SPAN` | Elemento Span | Contenedor en línea `<span>` |
| **32** | `L32-CLOSE-SPAN` | Cerrar etiqueta Span | Cierre de etiqueta `</span>` |
| **33** | `L33-UL` | Lista desordenada | Contenedor de lista con viñetas `<ul>` |
| **34** | `L34-LI` | Elemento de lista | Elemento `<li>` |
| **35** | `L35-CLOSE-LI` | Cerrar elemento de lista | Cierre de etiqueta `</li>` |
| **36** | `L36-OL` | Lista ordenada | Contenedor de lista numerada `<ol>` |
| **37** | `L37-CLOSE-UL` | Cerrar lista desordenada | Cierre de etiqueta `</ul>` |
| **38** | `L38-CLOSE-OL` | Cerrar lista ordenada | Cierre de etiqueta `</ol>` |

### Fase 5: Intermedio y avanzado (Pisos 39–48)
| Piso | Código | Título | Tarea / Concepto |
| :---: | :--- | :--- | :--- |
| **39** | `L39-FORM` | Contenedor de formulario | Envoltorio de entrada `<form>` |
| **40** | `L40-CLOSE-FORM` | Cerrar etiqueta de formulario | Cierre de etiqueta `</form>` |
| **41** | `L41-INPUT` | Campo de entrada | Campo autocerrado `<input>` |
| **42** | `L42-TABLE` | Tabla de datos | Contenedor `<table>` |
| **43** | `L43-TR` | Fila de tabla | Elemento de fila `<tr>` |
| **44** | `L44-TD` | Celda de tabla | Elemento de celda de datos `<td>` |
| **45** | `L45-CLOSE-TABLE` | Cerrar etiqueta de tabla | Cierre de etiqueta `</table>` |
| **46** | `L46-COMMENT` | Comentarios HTML | Sintaxis `<!-- comment -->` |
| **47** | `L47-CLASS` | Atributo Class | Destino de estilo `class="..."` |
| **48** | `L48-ID` | Atributo ID | Destino único `id="..."` |

### Fase 6: Desafío final (Pisos 49–51)
| Piso | Código | Título | Tarea / Concepto |
| :---: | :--- | :--- | :--- |
| **49** | `L49-DOCTYPE` | Tipo de documento | Declaración `<!DOCTYPE html>` |
| **50** | `L50-META-CHARSET` | Codificación de caracteres | Metadatos `<meta charset="UTF-8">` |
| **51** | `L51-COMPLETE` | **JEFE FINAL (FINAL BOSS)** | Construye una página web completa y válida |

---

## 🔑 Sistema de progresión por códigos de nivel

En lugar de depender de las API de almacenamiento del navegador (`localStorage`, `indexedDB` o cookies), el progreso se guarda mediante **Códigos de nivel (Level Codes)** cortos y legibles por humanos.

### Cómo funciona
1. Al completar un piso, la aplicación muestra un código único (por ejemplo, `L5-PARA`).
2. Los usuarios pueden copiar, guardar o anotar el código.
3. En sesiones posteriores, ingresar el código en el campo **JUMP TO FLOOR** (IR AL PISO) carga instantáneamente el estado de ese piso.

### Beneficios
- **Multi-navegador y multi-dispositivo**: Cambia sin problemas entre un teléfono móvil antiguo y una computadora de escritorio.
- **Huella de privacidad cero**: Funciona sin rastrear usuarios, almacenar cookies ni realizar solicitudes web.
- **Sin dependencias de API**: Funciona en navegadores creados antes de que existieran las especificaciones de almacenamiento local.

---

## 🛠️ Pautas de personalización y extensión

Debido a que toda la lógica de la aplicación se almacena en una matriz de JavaScript limpia, agregar o modificar pisos requiere editar la matriz `levels` dentro de `index.html`.

### Agregar un nuevo piso

```javascript
{
    id: "L52-HEADER",
    title: "Floor 52: Header Semantic Element",
    info: "The <header> tag represents introductory content or navigation links.",
    hint: "Type <header> to open the header section.",
    desc: "Create an opening header tag.",
    check: function(input) {
        var clean = input.toLowerCase().replace(/\s+/g, '');
        return clean.indexOf("<header>") !== -1;
    }
}

Pautas de diseño de validación
Al agregar reglas de validación, mantén las reglas de compatibilidad universal del proyecto:
 * Usa operaciones de cadena estándar: Confía en métodos como .indexOf(), .toLowerCase() y expresiones regulares básicas.
 * Maneja los espacios en blanco de forma flexible: Evita comparaciones de cadenas estrictas que fallen debido a espacios adicionales al final o saltos de línea.
 * Preserva la compatibilidad: No introduzcas métodos de ES6 (como .includes()) a menos que tengan un polyfill integrado de forma nativa dentro del archivo.
🌍 Progreso de traducción de idiomas
> Descargo de responsabilidad: Las traducciones de idiomas en este proyecto se generan utilizando Inteligencia Artificial (IA). Si bien los modelos de IA proporcionan procesamiento de alta calidad, pueden existir errores contextuales menores.
> 
Nuestro objetivo es respaldar los principales idiomas del mundo hablados por más de 1 millón de personas.
Idiomas principales
 * [x] Inglés (English)
 * [x] Alemán (Deutsch)
 * [x] Chino - Mandarín (普通话)
 * [x] Hindi (हिन्दी)
 * [x] Español (Español)
 * [x] Árabe - Estándar moderno (العربية الفصحى)
 * [o] Francés (Français)
 * [o] Bengalí (বাংলা)
 * [o] Portugués (Português)
 * [o] Ruso (Русский)
 * [o] Urdu (اردو)
 * [o] Indonesio (Bahasa Indonesia)
 * [o] Suajili (Kiswahili)
 * [o] Hausa (Harshen Hausa)
 * [o] Yoruba (Èdè Yorùbá)
 * [o] Zulú (isiZulu)
 * [o] Twi (Akan)
 * [o] Japonés (日本語)
 * [o] Punyabi (ਪੰਜਾਬੀ / پنجابی)
 * [o] Vietnamita (Tiếng Việt)
 * [o] Turco (Türkçe)
 * [o] Coreano (한국어)
(Leyenda: [x] Completado | [o] En curso | [ ] Planificado)
📐 Especificaciones técnicas
 * Formato de archivo: Archivo único .html (~50 KB)
 * Estándares: HTML5, CSS3, ES3/ES5 JavaScript
 * Dependencias: 0 bibliotecas externas, 0 fuentes, 0 frameworks
 * Requisito de red: 0 KB/s (funcional 100% sin conexión)
 * Requisitos de almacenamiento: Ninguno
 * Requisitos mínimos del navegador: Internet Explorer 6+, Firefox 1.0+, Safari 1.0+, Chrome 1.0+, o cualquier navegador WebKit/Gecko antiguo.
📄 Licencia y autor
Autor
M-Tarantino (@M-Tarantino)
Licencia
Este proyecto está licenciado bajo la Licencia MIT. Eres libre de usar, modificar, distribuir, alojar y enseñar con este software tanto para fines comerciales como no comerciales, siempre que se conserve la atribución original.
Tower of HTML — Accesible. Duradero. Universal.

