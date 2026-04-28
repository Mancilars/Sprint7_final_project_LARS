# Proyecto: Análisis de Clientes y Uso - ConnectaTel

## Objetivo del Proyecto

Este proyecto tiene como objetivo analizar el comportamiento de los usuarios de ConnectaTel a partir de sus patrones de uso (llamadas y mensajes), con el fin de identificar segmentos de clientes, detectar problemas de calidad en los datos y generar insights accionables para la toma de decisiones de negocio.

---

## Datasets Utilizados

Se utilizaron los siguientes datasets:

- **users**: información de los clientes (edad, ciudad, plan, fecha de registro y churn).
- **usage**: registros de uso del servicio (tipo de interacción, duración, longitud y fecha).
- **plans**: catálogo de planes disponibles (Básico y Premium).

---

## Etapas del Análisis

1. **Exploración de datos**
   - Revisión de estructura, tipos de variables y consistencia general.

2. **Calidad de datos**
   - Identificación de valores nulos.
   - Detección de sentinels (ej. -999 en edad, “?” en ciudad).
   - Revisión de fechas fuera de rango.

3. **Limpieza de datos**
   - Reemplazo de valores inválidos.
   - Tratamiento de nulos.
   - Corrección de fechas no válidas.

4. **Transformación de datos**
   - Creación de variables de uso (mensajes, llamadas, minutos).
   - Agregación por usuario.
   - Unión de datasets mediante `merge`.

5. **Análisis exploratorio**
   - Estadísticas descriptivas.
   - Visualización de distribuciones.
   - Identificación de outliers con método IQR.

6. **Segmentación de clientes**
   - Segmentación por nivel de uso (Bajo, Medio, Alto).
   - Segmentación por edad (Joven, Adulto, Adulto Mayor).

7. **Insights de negocio**
   - Interpretación de resultados.
   - Recomendaciones estratégicas basadas en comportamiento del usuario.

---

## Cómo ejecutar el notebook

### Opción 1: Google Colab (recomendado)

1. Abrir Google Colab.
2. Subir el archivo `.ipynb`.
3. Subir los datasets (`users`, `usage`, `plans`) al entorno.
4. Ejecutar las celdas en orden.

### Opción 2: Jupyter Notebook (local)

1. Instalar dependencias:
   ```bash
pip install pandas numpy matplotlib seaborn
2. Abrir el notebook con Jupyter.
3. Ejecutar todas las celdas de arriba hacia abajo.

## Guía de Reproducción

Cargar los datasets originales.
Realizar limpieza de datos (nulos, sentinels y fechas).
Generar variables de uso por usuario.
Unir datasets para crear user_profile.
Realizar análisis exploratorio (estadísticos y visualizaciones).
Detectar y analizar outliers con método IQR.
Crear segmentaciones de clientes.
Generar insights finales y conclusiones.

## Conclusión
El análisis permitió identificar que la mayoría de usuarios tiene un bajo nivel de uso, mientras que un grupo reducido concentra el consumo intensivo del servicio. Esto abre oportunidades claras de segmentación y optimización de planes para mejorar la estrategia comercial de ConnectaTel.
