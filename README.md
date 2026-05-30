# Vamos a crear el archivo README.md completo usando código Python para que quede grabado en el sistema
# y se incluyan de forma exacta las referencias de las herramientas (DBeaver, SQL, Power BI) y las imágenes correspondientes.

readme_code_content = """# 📊 Dashboard de Operaciones - Call Center Hospitalario de Urgencias

Este repositorio contiene un proyecto completo de **Analítica e Ingeniería de Datos (End-to-End)** enfocado en la optimización operativa de un servicio de atención telefónica hospitalaria de urgencias. El ciclo de vida abarca desde la conexión al motor de base de datos y la limpieza de datos por medio de SQL, hasta el modelado analítico mediante expresiones DAX y la maquetación de un cuadro de mando ejecutivo interactivo.

---

## 🛠️ Arquitectura y Herramientas Utilizadas

* **DBeaver (Community Edition):** Utilizado como cliente de base de datos multomotor para gestionar las conexiones de datos, configurar la codificación (`UTF-8`), definir el mapeo de tablas (`Tables mapping`) e importar masivamente la fuente de datos.
* **SQL (Limpieza y Estructuración):** Implementación de scripts para la normalización de tipos de datos, inspección de variables clave y aseguramiento de la consistencia e integridad de la información en una vista limpia (`call_center_hospital_limpio`).
* **Power BI Desktop:** Capa de visualización, modelado relacional y desarrollo de lógica de negocio interactiva mediante **DAX (Data Analysis Expressions)**.

---

## 🔄 Fases del Desarrollo e Integración

### 1. Extracción e Importación de Datos (DBeaver)
Se estructuró el entorno de base de datos mediante **DBeaver**, parametrizando el delimitador de columnas, la posición de los encabezados de la tabla original y forzando la codificación de caracteres en formato universal compatible con analítica avanzada.
