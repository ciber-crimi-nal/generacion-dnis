# 🆔 Generación Sintética de Documentos Nacionales de Identidad

Este proyecto presenta una metodología para la generación automática de **Documentos Nacionales de Identidad (DNI)** sintéticos, con el objetivo de crear **conjuntos de datos realistas y anónimos** que puedan ser utilizados en investigación, desarrollo y entrenamiento de sistemas de detección de falsificaciones.

---

## 🎯 Objetivos

- Simular **perfiles biográficos completos** de ciudadanos españoles.
- Generar documentos DNI sintéticos con estructura y formato realista.
- Automatizar el proceso de creación de:
  - Fotografías frontales válidas
  - Datos personales y de soporte
  - Firmas manuscritas sintéticas
  - Representación gráfica sobre soporte del DNI

---

## ⚙️ Metodología

### Evaluación de características faciales

El sistema comienza con la generación de imágenes de rostros sintéticos a través de redes generativas adversarias (GANs). Cada imagen se analiza automáticamente mediante métricas faciales que permiten:

- Evaluar expresividad, frontalidad, nitidez, exposición y posición
- Calificar cada imagen en una escala de 0 a 100
- Asegurar el cumplimiento de la normativa española (Real Decreto 1553/2005)

> Las imágenes que no superan los umbrales definidos son descartadas automáticamente.

### Generación del perfil biográfico

A partir de la imagen aceptada se genera el perfil biográfico:

- **Edad y sexo** estimados con red neuronal
- **Nombre, apellidos, progenitores** y demás datos personales generados a partir de bases del INE
- **Firma sintética** generada usando fuentes tipográficas que simulan trazos manuscritos
- **Datos del soporte** (número de soporte, equipo de expedición, fechas...) generados aleatoriamente con formatos válidos

### Composición del documento

Todos los elementos del perfil se integran sobre un **soporte gráfico base del DNI**, respetando posiciones, tipografías y dimensiones. El proceso incluye:

- Inserción de fotografía procesada (sin fondo, escala de grises, difuminada)
- Inserción de texto en formato y posición realista
- Representación de zona de lectura mecánica (OCR-B, estándar ICAO 9303)
- Inserción de firma
- Aplicación de efectos visuales (ruido, desenfoque, holograma)

---

## 🧪 Resultados esperados

- Conjuntos de datos sintéticos de DNIs indistinguibles de ejemplos reales (excepto por elementos de seguridad física).
- Documentos válidos para entrenar modelos de:
  - Detección de falsificaciones
  - Detección de documentos sintéticos
  - Evaluación automática de calidad de imagen facial

---

## 📚 Recursos y datasets
- 🔗 [ThisPersonDoesNotExist](https://thispersondoesnotexist.com/)
- 📊 [INE: nombres y apellidos frecuentes](https://www.ine.es/)
- 🔤 Tipografía OCR-B e ISO 1073-2 para zona de lectura automática

## 🏛 Equipo y Financiación
> Victoria Amores Chaparro [vicamoresc@unex.es](mailto:vicamoresc@unex.es), Fernando Broncano Morgado [fbroncano@unex.es](mailto:fbroncano@unex.es), Álvaro Hernández Martín [ahernandez@mobbeel.com](mailto:ahernandez@mobbeel.com), Óscar Mogollón Gutiérrez [oscarmg@unex.es](mailto:oscarmg@unex.es), Alberto López Trigo [albertolt@unex.es](mailto:albertolt@unex.es), José Carlos Sancho Núñez [jcsanchon@unex.es](mailto:jcsanchon@unex.es), Sebastião Pais [sabastiao@di.ubi.pt](mailto:sabastiao@di.ubi.pt).

Esta iniciativa se realiza en el se realiza en el marco de los fondos del Plan de Recuperación, Transformación y Resiliencia, financiados por la Unión Europea (Next Generation) - Instituto Nacional de Ciberseguridad (INCIBE) en el proyecto C108/23 “Detección de Falsificación de Documentos de Identidad mediante Técnicas de Visión por Computador e Inteligencia Artificial”. Los autores agradecen la colaboración de la empresa Mobbeel Solutions S.L. por su generoso apoyo, su compromiso con la investigación y la asistencia técnica realizada en el desarrollo de este trabajo.
![BandaLogos_INCIBE_es-100](https://github.com/user-attachments/assets/a2290f37-69d9-4caf-bee1-2b29c47bac97)
