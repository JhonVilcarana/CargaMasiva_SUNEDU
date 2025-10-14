# 🚀 Automatización de Carga masiva para SUNEDU con Python

Este proyecto automatiza la **limpieza, validación y estandarización de datos institucionales** para su envío masivo a **SUNEDU**, evitando la carga manual registro por registro.  
El proceso transforma los datos provenientes del sistema académico en archivos listos para carga, conforme a las **plantillas oficiales** de SUNEDU para **Postulantes, Matriculados y Egresados**.

---

### 🎯 El Problema

Antes, preparar estos informes era un proceso **manual, repetitivo y muy lento**. El personal debía tomar los datos de los estudiantes (postulantes, matriculados y egresados) y convertirlos a mano al formato exacto que exige SUNEDU. Esto implicaba:

* **Convertir texto a códigos:** Cambiar manualmente "DNI" por el código `1`, "Maestría en Educación" por `230`, o "Perú" por `9233`.
* **Corregir errores:** Arreglar uno por uno los números de DNI mal escritos, las fechas en formato incorrecto o los datos que faltaban.
* **Aplicar reglas complicadas:** Asegurarse de que cada tipo de estudiante (de segunda especialidad, maestría y doctorado) cumpliera con reglas específicas para no ser rechazado.

Este trabajo tomaba **horas**, era muy propenso a errores y causaba que los informes fueran rechazados, obligando a empezar todo de nuevo.

---

### 💡 La Solución

Para solucionar esto, desarrollé unos **scripts en Python** que hacen todo el trabajo pesado de forma automática. La herramienta funciona en tres simples pasos:

1.  **Lee el archivo Excel:** Toma el reporte tal como sale del sistema de la universidad.
2.  **Limpia y Transforma los Datos:**
    * **Corrige y valida** la información automáticamente (fechas, documentos, etc.).
    * **Traduce** todo el texto a los códigos oficiales de SUNEDU en segundos.
    * **Rellena inteligentemente** la información que falta. Por ejemplo, si un estudiante no tiene un correo registrado, el programa se lo crea basándose en su nombre y apellido.
3.  **Genera el Archivo Final:** Crea una nueva versión del Excel, perfectamente formateada y lista para ser enviada a SUNEDU sin ninguna revisión manual.

---

### ✨ El Impacto

Esta herramienta transformó por completo el proceso:

* ✅ **Eficiencia Total:** Redujo el tiempo de preparación de **horas a menos de un minuto**.
* 🎯 **Cero Errores:** Eliminó los errores humanos, asegurando que los datos son siempre correctos.
* ⚖️ **Cumplimiento Asegurado:** Ayudó a la universidad a ponerse al día con informes que estaban pendientes desde 2020, eliminando riesgos de sanciones.

---

## ⚙️ Tecnologías utilizadas

- 🐍 **Python 3.x**  
- 📊 **pandas**  
- 📗 **openpyxl**  
- 🧮 **numpy**  
- 🧰 **re** (expresiones regulares)
