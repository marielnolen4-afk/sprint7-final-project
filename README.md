Análisis de Comportamiento de Clientes – ConnectaTel
El objetivo de este proyecto es analizar el comportamiento de los clientes de ConnectaTel, una empresa de telecomunicaciones en Latinoamérica, para:
Entender patrones de uso de llamadas y mensajes.
Identificar segmentos de clientes según edad y nivel de uso.
Detectar outliers y clientes de alto valor.
Proponer recomendaciones de mejora en la oferta de planes y estrategias de retención.

Los datasets utilizados plans.csv – Información de los planes disponibles:- Precio, minutos incluidos, GB incluidos, costo por extras.
users.csv – Información de los clientes: - Edad, ciudad, fecha de registro, plan asignado, churn.
usage.csv – Detalle del uso real de servicios: - Cantidad de llamadas, mensajes, duración, fecha de uso, tipo de servicio (call/text).

Etapas del análisis realizadas:
Exploración de datos
   - Revisión de columnas numéricas y categóricas.
   - Identificación de valores nulos y sentinels.
Limpieza de datos
   - Reemplazo de valores inválidos (`-999` en edad, `?` en ciudad).
   - Corrección de fechas fuera de rango.
Agregación y creación de variables
   - Agregado de `usage` por usuario.
   - Creación de variables auxiliares: `cant_mensajes`, `cant_llamadas`, `cant_minutos_llamada`.
   - Segmentación de clientes: `grupo_uso` y `grupo_edad`.
Visualización
   - Histogramas y boxplots para distribuciones y outliers.
   - Countplots por grupo de uso y edad.
Análisis de segmentos
   - Identificación de clientes más valiosos según uso y plan.
   - Detección de patrones de consumo extremo (outliers).
 Recomendaciones
   - Sugerencias para nuevos planes y campañas segmentadas.
   - Estrategias de retención de clientes Premium y heavy users.

   - Cómo ejecutar el notebook
     Clonar o descargar este repositorio.
     Abrir el notebook `ConnectaTel_Analisis.ipynb` en Google Colab o Jupyter Notebook.
     Asegurarse de tener instaladas las librerías necesarias: bash pip install pandas numpy matplotlib seaborn
     Cargar los datasets (users.csv, usage.csv, plans.csv) en el mismo directorio o subirlos a Colab.
     Ejecutar las celdas paso a paso siguiendo las instrucciones del notebook.

     Guía de reproducción
Limpieza de datos: corregir valores nulos, sentinels y fechas imposibles.
Creación de variables agregadas y segmentación (grupo_uso y grupo_edad).
Visualización de distribuciones y outliers para análisis exploratorio.
Interpretación de segmentos y clientes de alto valor.
Aplicar recomendaciones basadas en los patrones detectados.
