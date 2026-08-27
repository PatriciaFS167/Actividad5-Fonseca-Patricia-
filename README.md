# Actividad5-Fonseca-Patricia-

# Validación de Categorización de Docentes de un Programa Académico

**Autor:** Patricia Fonseca Sánchez  
**Proyecto:** Actividad 5 – Análisis e Integración de Datos Académicos  

## Descripción del Proyecto
Este estudio de caso tiene como objetivo validar la categorización de los docentes pertenecientes a un programa académico mediante la integración y el cruce de dos fuentes de datos principales:

1. **Base de Datos Institucional:** Listado oficial de docentes del programa académico, identificados por su número de documento.
2. **Base de Datos de Minciencias:** Registro oficial de resultados de categorización de investigadores.

Mediante este análisis se determina qué docentes cuentan con una categoría vigente en Minciencias, cuáles no registran información y cómo se distribuyen las distintas categorías encontradas. Esta información constituye una herramienta clave para la gestión institucional en la presentación de proyectos a convocatorias.

---

## Objetivos del Proyecto

- **Objetivo Principal:** Validar la correspondencia entre la base institucional de docentes y la información de categorización de Minciencias utilizando **Python** y **Pandas**, generando indicadores de cobertura e informes visuales.
- **Objetivos Específicos:**
  - Limpiar e inspeccionar la calidad de la información (tratamiento de registros duplicados).
  - Unificar estructuras mediante la estandarización y renombrado de variables.
  - Ejecutar un cruce de datos (`merge`) tomando como llave el número de documento del docente y conservando el universo institucional.
  - Imputar valores faltantes e indicar la distribución de categorías.

---

## Flujo del Proceso de Análisis

1. **Exploración de Datos:** Lectura y verificación de la estructura y calidad de las bases.
2. **Limpieza de Datos:** Identificación y eliminación de registros duplicados en la base institucional.
3. **Estandarización:** Renombrado de las variables de interés (ej. categorías).
4. **Cruce de Información:** Combinación de bases mediante un *Left Join* tomando como llave principal el número de documento.
5. **Generación de Indicadores y Tratamiento de Nulos:** Reemplazo de datos ausentes por la etiqueta `N.A.` y cálculo de la cobertura de docentes categorizados.
6. **Exportación y Visualización:** Generación de archivos de salida estructurados y representaciones gráficas del estado de categorización.

---

## Retos y Líneas de Trabajo Futuras

El modelo desarrollado se puede complementar integrando fuentes de datos adicionales (convocatorias activas, datos demográficos, tipo de vinculación, pertenencia a grupos de investigación y producción científica en la plataforma SCIENTI).

Esta integración permitirá avanzar hacia:

- **Optimización de Recursos:** Reducción de reprocesos administrativos para docentes e investigadores, optimizando tiempos y costos operativos.
- **Calidad de la Información:** Mantenimiento de un registro actualizado, veraz y centralizado de la producción científica.
- **Interoperabilidad Tecnológica:** Conexión eficiente entre los sistemas de gestión de investigación institucionales y la plataforma **SCIENTI** de Minciencias.
- **Impacto Institucional:** Incremento en la visibilidad de la universidad y mejor posicionamiento para la participación en convocatorias de financiación internas y externas.

---

## Tecnologías Utilizadas

- **Lenguaje:** Python 3
- **Librerías Principales:**
  - `pandas` (para manipulación, limpieza e integración de datos)
  - `matplotlib` / `seaborn` (para generación de visualizaciones)
- **Entorno de Desarrollo:** Jupyter Notebook / Google Colab
