# Call Center Hospital Analytics 📊

## 📋 Descripción del Proyecto
Este proyecto desarrolla un análisis integral de las operaciones del centro de contacto de una institución de salud. El objetivo principal es evaluar la eficiencia en el enrutamiento de llamadas, identificar cuellos de botella y proponer mejoras basadas en datos para la atención al usuario.

## 🛠️ Tecnologías Utilizadas
- **Python (Pandas & NumPy):** Utilizado para el proceso de extracción, limpieza, normalización y transformación del dataset sintético hospitalario (ETL).
- **SQL:** Consultas de agregación y segmentación de datos para agrupar métricas por horas, tipos de llamadas y estados de resolución.
- **Power BI:** Diseño e implementación de un dashboard interactivo enfocado en KPIs de gestión hospitalaria.

## 📈 Métricas y Hallazgos Analizados
A través del desarrollo de scripts y visualizaciones, el proyecto se enfoca en resolver:
- **Volumen de llamadas e identificación de Horas Pico:** Para optimizar la distribución del personal administrativo y médico en las franjas horarias críticas.
- **Tiempos de Espera y Abandono:** Análisis de llamadas perdidas frente a la capacidad de respuesta operativa del centro médico.
- **Eficiencia de Enrutamiento:** Evaluación de las derivaciones a diferentes áreas (citas, urgencias, información general) para agilizar el flujo de atención.

## 🚀 Cómo Ver el Proyecto
1. El procesamiento y limpieza de datos se encuentra documentado en los scripts de Python dentro del repositorio.
2. Las conclusiones estratégicas están orientadas a optimizar la toma de decisiones en la gestión de recursos de salud.
---

## 🔄 El Proceso Técnico Paso a Paso (ETL)

El desarrollo del proyecto se ejecutó siguiendo las fases del ciclo de vida tradicional del manejo de datos:

### 1. Conexión y Migración (DBeaver)
La base del proyecto se estructuró parametrizando el asistente de transferencia de datos en **DBeaver**. Se configuró rigurosamente el formato de codificación en **`UTF-8`**, se definió la posición de las cabeceras de las columnas y el delimitador de campos para asegurar una ingesta sin pérdida de caracteres especiales.
![Datos_limpios_de Operaciones Hospitalarias Urgencias](Dbeaver_datos_limpios.png)

## 📈 Dashboard Gerencial e Insights de Operación

Configuracion 
![Configuracion de Dashboard de Operaciones Hospitalarias Urgencias](Powebi.png)

El lienzo final del tablero fue maquetado bajo una distribución ejecutiva limpia y funcional, permitiendo que todos los elementos visuales se recalculen automáticamente mediante el uso de un segmentador por Estado federado (`State`).
![Dashboard de Operaciones Hospitalarias Urgencias](Reporte_powerbi.png)

### 💡 Hallazgos Críticos de Negocio (Insights):
* **Canales Críticos:** El canal de contacto telefónico directo (`Phone`) representa el núcleo de la demanda.
  
#### 🕒 2. Patrones Cíclicos de Horas Pico (Saturación)
El análisis del volumen temporal basado en la columna calculada `Hora_Dia` demostró que la demanda del centro de salud no es lineal ni constante a lo largo de la jornada, revelando picos y valles operativos críticos para la planeación del personal:

* **Pico Crítico Principal (Madrugada):** Se sitúa de forma contraintuitiva en las primeras horas de la noche y madrugada (específicamente entre las **0:00 y las 3:00 am**), registrando volúmenes que superan las 440 llamadas por hora.
* **Pico Secundario (Tarde):** Se presenta a mitad de la tarde, concretamente entre las **3:00 pm y 4:00 pm (horas 15 y 16)**.
* **Valle de Demanda:** El punto con menor actividad y saturación en las líneas telefónicas se registra sobre las **6:00 am**.
