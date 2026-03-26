# **Proyecto: Análisis de Eficacia de Operadores — CallMeMaybe**

Este proyecto se centra en el análisis de datos para identificar operadores ineficaces en el servicio de telefonía virtual CallMeMaybe. A través de un análisis exploratorio de datos (EDA) y pruebas estadísticas, se evalúan métricas clave como tasas de llamadas perdidas, tiempos de espera prolongados y proporción de llamadas salientes por operador. El objetivo es proporcionar a los supervisores información para mejorar la eficiencia operativa y la calidad del servicio.

**Objetivo**

El proyecto se estructura en las siguientes fases principales:

1. **Validación y Limpieza de Datos:** Preparar y validar los datasets de llamadas y clientes.
2. **Análisis de Calidad de Datos:** Evaluar la integridad y distribución de los datos.
3. **Análisis Exploratorio de Datos:** Explorar distribuciones, tendencias y métricas por operador.
4. **Identificación de Operadores Ineficaces:** Clasificar operadores basados en criterios de ineficacia.
5. **Análisis Detallado de Operadores:** Profundizar en el rendimiento de operadores específicos.
6. **Pruebas de Hipótesis Estadísticas:** Validar diferencias estadísticamente significativas.
7. **Conclusiones y Recomendaciones:** Sintetizar hallazgos y proponer estrategias de intervención.

**🛠️ Tecnologías Utilizadas**

* **Python:** Lenguaje principal para el análisis de datos.
* **Pandas:** Para la manipulación, limpieza y agregación de datos.
* **NumPy:** Para operaciones numéricas y manejo de arrays.
* **Matplotlib y Seaborn:** Para la visualización de datos, incluyendo gráficos de distribución, boxplots y análisis por operador.
* **SciPy:** Para la realización de pruebas estadísticas (prueba de Mann-Whitney U).
* **Jupyter Notebook:** Entorno interactivo para el desarrollo del análisis.

**Pasos Clave**

1. **Validación y Limpieza de Datos:**
   - Se cargaron los datasets `telecom_dataset_new.csv` (registros de llamadas) y `telecom_clients_us.csv` (información de clientes).
   - Se realizó limpieza de datos, conversión de tipos y filtrado por período relevante.

2. **Análisis de Calidad de Datos:**
   - Se evaluó la distribución de llamadas por operador, dirección y tipo.
   - Se verificó la integridad de los datos y se identificaron valores atípicos.

3. **Análisis Exploratorio de Datos:**
   - Se exploraron métricas como duración de llamadas, tiempos de espera y tasas de pérdida.
   - Se visualizaron distribuciones y tendencias temporales.

4. **Identificación de Operadores Ineficaces:**
   - Se definieron criterios: alta tasa de llamadas perdidas, tiempo de espera prolongado, baja proporción de llamadas salientes.
   - Se clasificaron operadores en eficaces e ineficaces.

5. **Análisis Detallado de Operadores:**
   - Se analizó el rendimiento de operadores individuales, incluyendo estadísticas descriptivas.
   - Se identificaron patrones de ineficacia.

6. **Pruebas de Hipótesis Estadísticas:**
   - Se aplicó la prueba de Mann-Whitney U para comparar grupos eficaces e ineficaces.
   - Se evaluó la significancia estadística de las diferencias.

7. **Conclusiones y Recomendaciones:**
   - Se sintetizaron hallazgos y se propusieron estrategias de intervención priorizadas.

**Resultados**

El análisis revela que:

- **Calidad de Datos:** Datasets limpios con registros de llamadas y clientes, cubriendo un período específico.
- **Identificación de Ineficaces:** 505 operadores (61.2% de la fuerza laboral) clasificados como ineficaces, basados en criterios de pérdida alta, espera prolongada, inconsistencia y baja salida.
- **Hallazgos Clave:** Riesgo de proceso (inconsistencia) afecta a 206 operadores; riesgo de servicio (tiempos) a 206; riesgo severo (múltiples problemas) a 147.
- **Top 10 de Riesgo:** Operadores con mayor ineficacia, dominados por inconsistencia extrema y tiempos de espera prolongados (hasta 1,007s).
- **Validación Estadística:** Prueba de Mann-Whitney U confirma diferencias significativas (p ≈ 0.0000).
- **Recomendaciones:** Estrategia segmentada: coaching inmediato para top 10, capacitación grupal para 147 de alto riesgo, auditoría para baja salida. Próximos pasos incluyen monitoreo post-intervención y ajuste de umbrales.

**Cómo Ejecutar el Proyecto**

1. Clona este repositorio en tu máquina local.
   ```bash
   git clone (https://github.com/ferchi4/Proyecto_spring_13)

2. Asegúrate de tener instaladas las dependencias necesarias:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy jupyter
   ```

3. Coloca los archivos de datos (`telecom_dataset_new.csv`, `telecom_clients_us.csv`) en el mismo directorio que el notebook.

4. Abre y ejecuta el archivo `Proy_Operadores.ipynb` en Jupyter Notebook.
   ```bash
   jupyter notebook Proy_Operadores.ipynb
   ```
