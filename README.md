# Challenge_telecomx
Analisis descriptivo de Telecom X

Desafios:

- Detectar los factores que llevan a la perdida de clientes ya que la tasa de cancelaciones.
- Recopilar
- Procesar
- Analizar datos
- Uso de diferentes bibliotecas
- Realizar modelos predictivos
- Desarrollar estrategias para disminuir la tasa de cancelacion


Actividades a practicar:

- Importar y manipular datos desde una API de manera eficiente.
- Aplicar los conceptos de ETL (Extracción, Transformación y Carga) en la preparación de los datos.
- Crear visualizaciones estratégicas para identificar patrones y tendencias.
- Realizar un Análisis Exploratorio de Datos (EDA) y generar un informe con insights relevantes.

Diccionario de Datos:

customerID: número de identificación único de cada cliente

Churn: si el cliente dejó o no la empresa

gender: género (masculino y femenino)

SeniorCitizen: información sobre si un cliente tiene o no una edad igual o mayor a 65 años

Partner: si el cliente tiene o no una pareja

Dependents: si el cliente tiene o no dependientes

tenure: meses de contrato del cliente

PhoneService: suscripción al servicio telefónico

MultipleLines: suscripción a más de una línea telefónica

InternetService: suscripción a un proveedor de internet

OnlineSecurity: suscripción adicional de seguridad en línea

OnlineBackup: suscripción adicional de respaldo en línea

DeviceProtection: suscripción adicional de protección del dispositivo

TechSupport: suscripción adicional de soporte técnico, menor tiempo de espera

StreamingTV: suscripción de televisión por cable

StreamingMovies: suscripción de streaming de películas

Contract: tipo de contrato

PaperlessBilling: si el cliente prefiere recibir la factura en línea

PaymentMethod: forma de pago

Charges.Monthly: total de todos los servicios del cliente por mes

Charges.Total: total gastado por el cliente

- Estado de Proyecto. En contruccion.

Ejecutar sistema.

```npm install react```


Informe Final

🔹 Introducción Este informe presenta el análisis del proyecto de Telecom X, una empresa que enfrenta una elevada tasa de cancelaciones de clientes. El objetivo fue identificar los factores que influyen en la evasión, generar información para diseñar modelos predictivos y proponer estrategias que fortalezcan la retención.

El proyecto se desarrolló bajo un proceso ETL para garantizar datos limpios y estructurados. Posteriormente, mediante un Análisis Exploratorio de Datos (EDA) se detectaron patrones, correlaciones y señales de riesgo asociadas al abandono.

🔹 Limpieza y Tratamiento de Datos

Los datos fueron extraídos desde una API en formato JSON e importados con Pandas, obteniendo un DataFrame sin procesar.

Se aplicó tratamiento de valores nulos y duplicados:

Eliminadas 11 filas con valores faltantes irreparables.

Reemplazadas 224 filas con el valor “Yes” para mantener consistencia en el análisis.

Se renombraron columnas al español para facilitar la interpretación y la comunicación con equipos no técnicos.

Se ajustaron los tipos de datos:

int64 para valores numéricos enteros.

float64 para cálculos.

str para valores categóricos.

Se tradujeron valores de filas para mayor claridad.

Se generó una nueva columna con el cálculo del valor diario de cada cliente para una visión más detallada.

🔹 Análisis Exploratorio de Datos (EDA)

Se calcularon métricas descriptivas (media, mediana, desviación estándar).

Se emplearon gráficos (matplotlib, seaborn y Plotly) para identificar patrones.

Principales hallazgos gráficos:

Pie chart: la tasa de churn es 28.8%.

Gráficos de barras: la mayoría de clientes tiene contratos de corto plazo y solo contrata servicios básicos (teléfono e Internet).

Boxplot, Violinplot y KDE:

Los clientes que cancelan lo hacen principalmente en los primeros 12 meses.

Cargos mensuales elevados están asociados a mayor riesgo de abandono.

Matriz de correlación: la duración del contrato es el factor con mayor peso en la retención.

🔹 Hallazgos Clave

28.8% de clientes abandonaron la empresa.

La duración del contrato es el factor más determinante en la permanencia.

Cargos mensuales altos aumentan ligeramente la probabilidad de fuga.

Contratar más servicios incrementa ingresos, pero no garantiza permanencia.

La mayor parte de bajas ocurre en los primeros 12 meses.

🔹 Conclusiones

El número de servicios contratados no asegura la retención. Lo decisivo son el tipo de contrato y el costo mensual.

Existe una correlación negativa entre churn y meses de contrato: a mayor tiempo en la empresa, menor probabilidad de fuga.

Aunque los cargos mensuales altos elevan el riesgo de abandono, los cargos totales altos reflejan en su mayoría clientes fieles de larga duración.

La venta cruzada aumenta ingresos, pero su éxito depende de ofrecer packs atractivos y precios competitivos.

El valor de vida del cliente depende tanto del número de servicios como de la longevidad del contrato.

🔹 Recomendaciones

Programas de fidelización temprana: enfocar esfuerzos en los primeros 12 meses con programas de bienvenida, llamadas de seguimiento y encuestas de satisfacción.

Incentivar contratos largos: ofrecer descuentos o beneficios adicionales en planes de 1-2 años frente a los contratos mensuales.

Optimización de precios: diseñar packs de servicios más económicos para disminuir la percepción de costos elevados.

Mejorar experiencia digital: fortalecer canales de soporte en facturación electrónica y optimizar la calidad del servicio de Internet (especialmente fibra óptica).

Ofrecer incentivos personalizados: detectar clientes con alta probabilidad de fuga y darles bonificaciones por extender el contrato.

🔹 Final Este análisis establece bases sólidas para implementar un sistema predictivo de abandono, mejorar estrategias de retención y optimizar la rentabilidad de Telecom X. La clave está en fomentar contratos de mayor duración, controlar la percepción de precios y reforzar la atención durante los primeros meses de relación con el cliente
