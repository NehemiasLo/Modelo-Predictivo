# Modelo-Predictivo
Modelo predictivo implementando regresión para predecir números, tome de ejemplo una base de datos midiendo la  satisfacción del cliente, para predecir según la edad y el tiempo de espera la satisfacción.

# ⚙️ acceso a la app

https://share.gemini.google/tKuV3gQ4bJ6y


# StatBlue Analytics 📊📈

StatBlue Analytics es una potente y sofisticada aplicación web interactiva desarrollada para el análisis estadístico descriptivo y modelado predictivo multivariable. Diseñada con una estética premium en tonos azul corporativo, la aplicación permite a analistas y tomadores de decisiones importar datos, explorar distribuciones, calcular estadísticos avanzados en tiempo real y simular escenarios futuros de forma 100% local y segura.

# 🌟 Características Principales

Lienzo desde Cero e Importación Inteligente (CSV/Excel): Inicio libre de datos para total flexibilidad. Integra la librería SheetJS para leer y procesar instantáneamente archivos de Excel (.xlsx, .xls) y de texto plano (.csv) de manera local en el navegador.

Gestión Dinámica de Datos (CRUD): Tabla interactiva para añadir, editar o eliminar registros manualmente. Cualquier modificación actualiza de inmediato toda la analítica gráfica e indicadores matemáticos.

Estadísticas Descriptivas de Alto Nivel: Cálculo automático en tiempo real de métricas de tendencia central y dispersión:

Tamaño de la Muestra ($N$) y Media.

Percentiles avanzados: Cuartil 1 ($Q1$/$P_{25}$), Mediana ($Q2$/$P_{50}$) y Cuartil 3 ($Q3$/$P_{75}$).

Desviación Estándar Muestral y Varianza.

Valores Máximos y Mínimos.

Formas de distribución: Asimetría (Skewness) y Curtosis de Fisher.

Visualizaciones de Alta Fidelidad (Chart.js):

Gráfico de Dispersión con Línea de Tendencia: Ajuste interactivo para analizar la correlación entre dos variables seleccionadas dinámicamente.

Histogramas de Frecuencia: Agrupación de datos en intervalos óptimos determinados matemáticamente mediante la Regla de Sturges.

Motor de Regresión Lineal Múltiple en JS Puro: Implementación nativa del método de Mínimos Cuadrados Ordinarios (MCO) para resolver ecuaciones del tipo $Y = \beta_0 + \beta_1 X_1 + \beta_2 X_2 + \dots$ sin dependencias del servidor.

Simulador Predictivo en Vivo: Controles deslizantes (sliders) generados de forma dinámica según las variables predictoras seleccionadas para realizar estimaciones inmediatas sobre la variable objetivo.

Asistente Inteligente de Satisfacción: Si el dataset contiene las variables Edad, Tiempo_Espera_Min y Puntaje_Satisfaccion, se activa un asistente de creación rápida que entrena un submodelo específico, proyecta la satisfacción en una escala estricta de 0 a 5 y muestra su exactitud ($R^2$).

# 🛠️ Stack Tecnológico

Frontend: HTML5, CSS3 con Tailwind CSS (Paleta personalizada Premium Blue).

Iconografía: Lucide Icons.

Visualización de Gráficos: Chart.js.

Motor de Hojas de Cálculo: SheetJS (xlsx) para análisis e interpretación local de archivos Excel.

Algoritmos Matemáticos: JavaScript puro (Álgebra lineal para resolución de ecuaciones normales y pivoteo parcial por eliminación Gauss-Jordan).

# 🤖 Desarrollo Asistido por IA

Este proyecto ha sido diseñado, estructurado y optimizado con la valiosa colaboración de Gemini (Google), quien asistió activamente en:

El planteamiento conceptual y la resolución matemática del motor de regresión lineal (MCO y eliminación Gauss-Jordan con pivoteo parcial) en JavaScript nativo.

La optimización del flujo interactivo y diseño responsivo de la interfaz de usuario con Tailwind CSS.

La depuración y estructuración del código bajo la arquitectura limpia de un solo archivo (Single-File Application).

# 📐 Fundamento Matemático del Motor Predictivo

El motor predictivo calcula el vector de coeficientes óptimos $\hat{\beta}$ utilizando la ecuación general de Mínimos Cuadrados Ordinarios (MCO):

$$\hat{\beta} = (X^T X)^{-1} X^T Y$$

Donde:

$X$ representa la matriz de características (variables predictoras) con una columna inicial de $1s$ para el intercepto ($\beta_0$).

$X^T$ es la transpuesta de la matriz de características.

$(X^T X)^{-1}$ representa la inversa de la matriz producto, resuelta mediante eliminación de Gauss-Jordan con pivoteo parcial para evitar fallos por singularidad.

$Y$ es el vector de observaciones de la variable objetivo.

El coeficiente de determinación ($R^2$), que representa la exactitud del modelo mostrada en la aplicación, se evalúa mediante:

$$R^2 = 1 - \frac{SS_{res}}{SS_{tot}}$$

Donde la suma de cuadrados de los residuos ($SS_{res}$) y la suma total de cuadrados ($SS_{tot}$) se determinan sobre la muestra completa en tiempo real.

# 🚀 Instalación y Ejecución

Al ser una aplicación basada puramente en el cliente (client-side), no requiere instalación de dependencias en el servidor ni configuraciones complejas de entorno (como Node.js o Python).

Descarga el archivo index.html.

Ábrelo directamente en tu navegador web de preferencia (Chrome, Edge, Firefox, Safari).

¡Listo! Sube tu archivo CSV/Excel o haz clic en "Cargar Datos de Prueba" para experimentar con la herramienta.

# 📁 Estructura del Archivo

El proyecto está diseñado bajo el patrón de Single-File Application, garantizando la portabilidad absoluta del sistema:

└── index.html       # Contiene todo el marcado HTML, estilos Tailwind, lógica JS y matemáticas matriciales.



# 🤝 Contribuciones

Las contribuciones son bienvenidas. Si encuentras algún problema o deseas añadir una mejora matemática o visual:

Haz un Fork del repositorio.

Crea una rama para tu mejora (git checkout -b feature/NuevaCaracteristica).

Realiza tus cambios y haz un Commit (git commit -am 'Agrega NuevaCaracteristica').

Haz Push a la rama (git push origin feature/NuevaCaracteristica).

Abre un Pull Request.

# 📄 Licencia

Este proyecto está bajo la Licencia MIT. Siéntete libre de utilizarlo, modificarlo y adaptarlo a tus necesidades corporativas o académicas.
