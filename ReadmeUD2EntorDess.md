Palabra del día: 29
Adrián Durán Durán


# Tarea Módulo 2: Reconocimiento de Elementos en el Desarrollo de un Programa Informático

**Asignatura:** Entorno de Desarrollo  
**Alumno:** Adrián Durán Durán  
**Fecha:** Octubre 2026  
**Proyecto:** NutriScan  

---

## 📌 1. Selección de la Aplicación

**Aplicación seleccionada:** NutriScan  

**Descripción del concepto:**  
NutriScan es una aplicación móvil diseñada para ayudar a personas con problemas alimenticios, intolerancias (como lactosa o fructosa) y alergias graves (como celiaquía). Su objetivo principal es simplificar la compra diaria en el supermercado para que el usuario no tenga que leer con detalle la letra pequeña de los ingredientes de cada producto.

**Justificación técnica:**
* **Usuarios principales y necesidad:** Los usuarios principales son personas celíacas, intolerantes a ciertos alimentos o sus familiares, que necesitan una respuesta rápida antes de comprar un producto en el punto de venta.
* **Modelo de desarrollo ágil:** Es ideal aplicar un modelo ágil (como Scrum) porque permite lanzar rápidamente un Producto Mínimo Viable (MVP) que detecte los alérgenos más comunes (gluten y lactosa) e ir añadiendo gradualmente nuevas alergias, bases de datos o funciones según el feedback de los usuarios.

---

## 📋 2. Listado de Características

A continuación se listan 10 características clave del sistema, clasificadas entre requisitos funcionales y no funcionales:

### Requisitos Funcionales (Funcionalidades del sistema)
1. **Configuración de perfil nutricional:** Permite registrar las alergias e intolerancias específicas del usuario.
2. **Escaneo de código de barras:** Utiliza la cámara del móvil para escanear el código y consultar el producto en la base de datos.
3. **Lector OCR de etiquetas:** Permite fotografiar la lista de ingredientes de un producto no catalogado para analizar el texto automáticamente.
4. **Sistema de alertas por semáforo:** Muestra un indicador visual en pantalla: Verde (apto), Amarillo (trazas/dudoso) y Rojo (no apto).
5. **Búsqueda manual de productos:** Incluye una barra de búsqueda por texto (nombre, marca o categoría) para consultas previas a la compra.

### Requisitos No Funcionales (Criterios de calidad)
6. **Rendimiento y velocidad:** El resultado tras el escaneo debe mostrarse en menos de 1.5 segundos.
7. **Usabilidad y diseño accesible:** Interfaz con botones amplios y alto contraste para facilitar su uso a cualquier perfil de persona.
8. **Modo fuera de línea (Offline):** Almacena una base de datos local en el dispositivo para funcionar en supermercados con mala cobertura.
9. **Seguridad y privacidad:** Cifrado y almacenamiento seguro local de los datos de salud e intolerancias del usuario.
10. **Disponibilidad del servidor:** El servicio en la nube debe mantener una disponibilidad del 99.9% para sincronizar novedades cuando haya conexión.

---

## 📄 3. Documentación Inicial

| Parámetro | Detalle |
| :--- | :--- |
| **Nombre de la Aplicación** | **NutriScan** (Nutrición + Escáner) |
| **Descripción Breve** | App móvil que analiza la seguridad alimentaria de los productos mediante escaneo de código de barras o lectura OCR de ingredientes. |
| **Objetivos** | Agilizar la compra en supermercados y evitar la ingesta accidental de alérgenos sin necesidad de leer manualmente las etiquetas. |
| **Usuarios Principales** | Personas celíacas, intolerantes a la lactosa/fructosa, alérgicas a frutos secos y familiares a cargo de su alimentación. |
| **Plataforma/s** | **Móvil Nivel Nativo (Android / iOS):** Permite el uso cómodo con una mano en el supermercado, acceso directo a la cámara y funcionamiento offline. |
| **Modelo Sugerido** | **Metodología Ágil (Scrum):** Desarrollo iterativo en Sprints de 2 semanas para entregas rápidas de valor e incorporación progresiva de alérgenos. |

---

## 🔍 4. Análisis de Requisitos

### Requisitos Funcionales (Qué debe hacer)

1. **Gestión y configuración del perfil nutricional:**  
   El sistema debe permitir seleccionar y editar las restricciones alimentarias específicas de cada usuario.  
   *Por qué es importante:* Es la base del sistema para personalizar el diagnóstico de cada alimento según las necesidades del usuario.

2. **Escaneo de código de barras de alimentos:**  
   La app debe capturar códigos de barras con la cámara para identificar automáticamente el producto en la base de datos.  
   *Por qué es importante:* Ahorra tiempo en el supermercado y evita errores al teclear los nombres de los productos manualmente.

3. **Lector de etiquetas por OCR (Reconocimiento Óptico de Caracteres):**  
   Permite tomar una foto a la lista de ingredientes impresa en envases no catalogados y extraer el texto para detectar alérgenos.  
   *Por qué es importante:* Mantiene la utilidad del software ante productos nuevos o ausentes en la base de datos central.

4. **Sistema de semaforización y alertas visuales:**  
   La interfaz debe mostrar un indicador claro inmediatamente tras el análisis: Verde (Apto), Amarillo (Trazas) o Rojo (No Apto).  
   *Por qué es importante:* Aplica el concepto de diseño centrado en el usuario, permitiendo tomar decisiones en un solo segundo.

5. **Sugerencia de alternativas aptas:**  
   En caso de detectar un producto No Apto (Rojo), la app debe mostrar un listado de productos alternativos compatibles.  
   *Por qué es importante:* Ofrece una solución completa al usuario en lugar de solo notificar el problema.

---

### Requisitos No Funcionales (Criterios de calidad)

1. **Rendimiento y tiempo de respuesta:**  
   El proceso completo de lectura y diagnóstico no debe superar los 1.5 segundos.  
   *Por qué es importante:* La eficiencia temporal es clave para evitar que el usuario abandone la app durante la compra.

2. **Usabilidad y accesibilidad:**  
   La interfaz debe permitir completar cualquier acción principal en un máximo de 3 toques de pantalla.  
   *Por qué es importante:* El perfil de usuario abarca desde jóvenes hasta personas mayores con poca experiencia tecnológica.

3. **Funcionamiento fuera de línea (Modo Offline):**  
   El sistema guardará localmente los productos más comunes para funcionar sin conexión activa a Internet.  
   *Por qué es importante:* Garantiza la fiabilidad en entornos reales como supermercados en sótanos o zonas rurales sin cobertura.

4. **Seguridad y privacidad de datos:**  
   Los datos sobre intolerancias y salud deben almacenarse de forma cifrada en el dispositivo.  
   *Por qué es importante:* La información de salud es sensible y su protección es crítica para mantener la confianza del usuario.

5. **Mantenibilidad y actualización de datos:**  
   El catálogo de ingredientes y productos debe actualizarse desde el servidor sin requerir una reinstalación completa de la app.  
   *Por qué es importante:* Permite escalar el sistema e incorporar nuevos productos de forma continua y transparente.

---

## 📹 5. Entrega y Presentación

* **Repositorio en GitHub:** [URL del Repositorio](https://github.com/ddadrian2006-alt/actv_entorno_de_desarrollo_ud2.2part.git)
* **Presentación / Vídeo:** *(Añadir enlace a YouTube si aplica)*
