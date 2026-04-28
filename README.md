# Proyecto: Análisis de Clientes y Uso - ConnectaTel

## Objetivo del Proyecto

Este proyecto tiene como objetivo analizar el comportamiento de los usuarios de ConnectaTel a partir de sus patrones de uso (llamadas y mensajes), con el fin de identificar segmentos de clientes, detectar problemas de calidad en los datos y generar insights accionables para la toma de decisiones de negocio.

---

## Datasets Utilizados

- **users**: información de clientes (edad, ciudad, plan, fechas).
- **usage**: registros de uso (llamadas, mensajes, duración, fecha).
- **plans**: catálogo de planes (Básico y Premium).

---

## Etapas del Análisis

- Exploración de datos  
- Calidad de datos (nulos, sentinels, fechas)  
- Limpieza de datos  
- Transformación y agregación por usuario  
- Análisis exploratorio  
- Segmentación de clientes  
- Visualización de resultados  
- Insights de negocio  

---

## Cómo ejecutar el proyecto

### Opción 1: Google Colab (recomendado)

1. Abrir Google Colab  
2. Subir el archivo `.ipynb`  
3. Subir los datasets (`users`, `usage`, `plans`)  
4. Ejecutar las celdas en orden  

---

### Opción 2: Jupyter Notebook (local)

Instalar dependencias:

```bash id="install_deps"
pip install pandas numpy matplotlib seaborn

Abrir el notebook en Jupyter y ejecutar todas las celdas de arriba hacia abajo.

---

## Guía de Reproducción

- Cargar datasets originales  
- Realizar limpieza de datos (nulos, sentinels y fechas)  
- Crear variables de uso por usuario  
- Generar tabla `user_profile`  
- Ejecutar análisis exploratorio  
- Detectar outliers con método IQR  
- Crear segmentaciones (uso y edad)  
- Generar visualizaciones finales  
- Interpretar resultados  

---

## Conclusión

El análisis muestra que la mayoría de los usuarios tiene un bajo nivel de uso del servicio, mientras que un grupo reducido concentra el consumo intensivo.

Esto representa una oportunidad clara para optimizar planes básicos, diseñar estrategias de activación y crear ofertas enfocadas en usuarios de alto consumo.
