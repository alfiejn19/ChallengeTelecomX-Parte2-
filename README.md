# ChallengeTelecomX-Parte2-
ChallengeTelecomX-Parte2- Solución

📋 Objetivo

Identificar los principales factores que influyen en la tasa de abandono de clientes (churn rate) que supera el 20%, desarrollando estrategias basadas en análisis predictivo para mejorar la retención.

🔧 Metodología

+ Tratamiento de Datos
+ Carga de datos: Importación del dataset desde repositorio GitHub
+ Limpieza inicial: Eliminación de columna ID por irrelevancia analítica
+ Verificación de calidad: Validación de integridad de datos
+ Balanceo: Aplicación de técnicas de oversampling para corregir desbalanceo en la variable objetivo

🎯 Análisis de Correlaciones

+ Variable objetivo: Churn
+ Selección de variables basada en correlación significativa
+ Establecimiento de umbral mínimo de correlación para inclusión de features
  
🧠 Modelado Predictivo

1. Implementación de KNN (K-Nearest Neighbors)

+ Estandarización de variables numéricas
+ Calibración óptima: 1 vecino con métrica Taxista (Manhattan)
+ Evaluación de performance: Sin evidencia de overfitting
+ Validación mediante matriz de confusión

2. Implementación de Random Forest

+ Procesamiento sin estandarización previa
+ Optimización de hiperparámetros: profundidad máxima de 9 niveles
+ Resultados consistentes sin sobreajuste
+ Desempeño comparativo con modelo KNN


📊 Hallazgos Principales

+ Factores críticos que incrementan el abandono:

    + 📅 Contratos de tipo mensual (alta rotación)
    + ⏳ Corta permanencia del cliente (<6 meses)
    + 💰 Costos mensuales y cargos diarios elevados
    + 🆕 Clientes nuevos con condiciones contractuales desfavorables
      
Variables más predictivas:
+ Tipo de contrato (month-to-month)
+ Meses de permanencia
+ Cargos mensuales
+ Costos diarios adicionales

  
🎯 Recomendaciones Estratégicas

+ Para clientes existentes

Migración progresiva de contratos mensuales a planes anuales
Programas de fidelización con beneficios escalonados
Revisión de estructura de costos para clientes de alto riesgo

+ Para nuevos clientes

Ofrecer costos diarios reducidos en contratos mensuales
Incentivos por adopción de contratos de mayor permanencia
Políticas de onboarding con condiciones promocionales


📈 Resultados y Performance

Ambos modelos predictivos demostraron capacidad efectiva para identificar patrones de abandono:

+ Modelo KNN: Mayor precisión en clasificación
+ Random Forest: Resultados consistentes con menor sobreajuste
+ Métricas de evaluación validadas mediante matrices de confusión
