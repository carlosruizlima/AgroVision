# 📊 Guía de Datos - Español

¡Bienvenido a la guía de datos de **AgroVision**! Este documento explica cómo trabajar con datos agrícolas en nuestro proyecto.

## Índice

- [Fuentes de Datos](#fuentes-de-datos)
- [Formatos de Datos](#formatos-de-datos)
- [Mejores Prácticas](#mejores-prácticas)
- [Ejemplos de Uso](#ejemplos-de-uso)

## Fuentes de Datos

### Datos Públicos Recomendados

1. **CONAB (Companhia Nacional de Abastecimiento)**
   - Series históricas de producción
   - Precios de materias primas
   - Enlace: https://www.conab.gov.br/

2. **IBGE (Instituto Brasileño de Geografía y Estadística)**
   - Datos demográficos y agrícolas
   - Estadísticas de producción
   - Enlace: https://www.ibge.gov.br/

3. **FAO (Organización de Alimentos y Agricultura)**
   - Datos globales de agricultura
   - Investigación y desarrollo
   - Enlace: https://www.fao.org/

### Datos Locales

- Registros de propiedades agrícolas
- Datos de sensores IoT
- Historiales de cosechas
- Análisis de suelos

## Formatos de Datos

### CSV (Valores Separados por Comas)

El formato recomendado para datos tabulares:

```csv
fecha,cultivo,produccion_kg,precio_unitario
2024-01-15,maíz,5000,0.85
2024-01-15,soja,3000,1.25
2024-01-16,maíz,4800,0.86
```

### JSON

Para datos estructurados y metadatos:

```json
{
  "propiedad": "Granja Solar",
  "cosecha": 2024,
  "cultivos": [
    {
      "nombre": "maíz",
      "area_hectareas": 50,
      "produccion_esperada_kg": 250000
    }
  ]
}
```

### Excel (XLSX)

Para análisis interactivos e informes.

## Mejores Prácticas

### 1. Limpieza de Datos

- Elimina valores faltantes (NaN)
- Estandariza formatos de fecha
- Corrige valores atípicos cuando sea necesario
- Valida tipos de datos

### 2. Documentación

Siempre documenta:
- Origen de los datos
- Fecha de recopilación
- Unidades de medida
- Valores faltantes

### 3. Sostenibilidad

- Utiliza datos de prácticas sostenibles
- Documenta impacto ambiental
- Registra uso de insumos
- Realiza seguimiento de indicadores de sostenibilidad

## Ejemplos de Uso

### Cargando datos con Python

```python
import pandas as pd

# Cargar datos de CSV
df = pd.read_csv('datos_agricultura.csv')

# Ver primeras filas
print(df.head())

# Estadísticas básicas
print(df.describe())
```

### Análisis Simple

```python
import pandas as pd

# Cargar datos
df = pd.read_csv('datos_agricultura.csv')

# Producción promedio por cultivo
produccion_promedio = df.groupby('cultivo')['produccion_kg'].mean()
print(produccion_promedio)

# Precio promedio
precio_promedio = df['precio_unitario'].mean()
print(f"Precio promedio: R$ {precio_promedio:.2f}")
```

## Estructura de Directorio de Datos

```
AgroVision/
├── data/
│   ├── raw/              # Datos brutos
│   ├── processed/        # Datos procesados
│   ├── examples/         # Datos de ejemplo
│   └── README.md         # Documentación de datos
```

## Seguridad y Privacidad

- Nunca compartas datos personales de agricultores
- Anonimiza información sensible
- Respeta la LGPD (Ley General de Protección de Datos)
- Documenta origen y uso de datos

---

**Versiones en otros idiomas:** [🇧🇷 Português](./data-guide.pt.md) | [🇬🇧 English](./data-guide.en.md)

¿Tienes preguntas? [Abre una Discussion](../../discussions)
