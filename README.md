# 📊 Análisis de Operaciones - Call Center Hospitalario de Urgencias

Este repositorio expone un proyecto completo de **Analítica e Ingeniería de Datos (End-to-End)** cuyo objetivo es auditar y optimizar el flujo operativo del servicio de atención telefónica de urgencias de un centro de salud, basándose en un histórico de **10,000 registros**. El pipeline abarca desde el aprovisionamiento en base de datos y limpieza con SQL, hasta el modelado analítico mediante expresiones DAX y el diseño de una interfaz ejecutiva interactiva en Power BI.

---

## 🛠️ Arquitectura de Herramientas

* **DBeaver (Community Edition):** Administrador de bases de datos utilizado para la gestión de conexiones de datos, mapeo de estructuras (`Tables mapping`) e importación controlada de grandes volúmenes de información.
* **SQL (Estructuración y Limpieza):** Implementación de reglas de negocio para la limpieza profunda, normalización de tipos de datos, corrección de inconsistencias e integridad en la tabla base `call_center_hospital_limpio`.
* **Power BI Desktop:** Motor analítico encargado del modelado conceptual, desarrollo de cálculos métricos mediante **DAX (Data Analysis Expressions)** y diseño de la interfaz visual dinámica.

---

## 🔄 El Proceso Técnico Paso a Paso (ETL)

El desarrollo del proyecto se ejecutó siguiendo las fases del ciclo de vida tradicional del manejo de datos:

### 1. Conexión y Migración (DBeaver)
La base del proyecto se estructuró parametrizando el asistente de transferencia de datos en **DBeaver**. Se configuró rigurosamente el formato de codificación en **`UTF-8`**, se definió la posición de las cabeceras de las columnas y el delimitador de campos para asegurar una ingesta sin pérdida de caracteres especiales.

```text
📸 [Imagen del Proceso: Configuración del entorno e importación de tablas en DBeaver]
Nombre del archivo en tu carpeta: dbeaver_setup.png (Referencia: <img width="1285" height="753" alt="image" src="https://github.com/user-attachments/assets/d1eccd4b-1e3f-472e-b548-428bf3ac5347" />
)
