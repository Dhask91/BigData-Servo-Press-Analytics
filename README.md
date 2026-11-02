# Big Data Servo Press Analytics

## Descripción del proyecto

Este proyecto implementa una arquitectura Big Data para la recopilación, procesamiento y análisis de datos generados por servo-prensas utilizadas en la manufactura de productos de la familia OR.

La solución permite analizar registros históricos de producción para evaluar diferentes programas de operación, identificar parámetros óptimos de trabajo y generar indicadores que apoyen la toma de decisiones dentro del proceso de manufactura.

---

## Objetivo

Desarrollar una plataforma basada en tecnologías Big Data capaz de:

- Capturar información generada por las servo-prensas.
- Procesar grandes volúmenes de registros históricos.
- Generar indicadores de calidad y desempeño.
- Apoyar la definición de rangos óptimos de operación.
- Reducir tiempos de ajuste y porcentaje de scrap.

---

## Problema de negocio

Actualmente, la definición de parámetros para nuevos programas de servo-prensas requiere múltiples pruebas y ajustes hasta encontrar valores que permitan mantener el producto dentro de tolerancia.

Esto puede generar:

- Incremento de scrap.
- Tiempo muerto de máquina.
- Consumo adicional de material.
- Incremento de costos de producción.

Los modelos OR28, OR40 y OR80 representan volúmenes de producción superiores a los 3 millones de piezas anuales, por lo que pequeñas mejoras en los parámetros de operación pueden generar beneficios significativos.

---

## Arquitectura implementada

```text
CSV OR28
    ↓
Apache Kafka
    ↓
Apache Spark
    ↓
PostgreSQL
    ↓
Power BI

Apache Airflow
(Orquestación)

Apache Hadoop HDFS
(Data Lake)
```

---

## Tecnologías utilizadas

- Python
- Apache Kafka
- Apache Spark
- Apache Hadoop HDFS
- PostgreSQL
- Power BI
- Apache Airflow
- Docker

---

## Variables analizadas

- Modelo
- Resultado (Pass/Fail)
- Displacement
- Max Force
- Time

---

## Indicadores obtenidos

| Indicador | Resultado |
|------------|-----------:|
| Total registros | 1500 |
| Piezas conformes | 1461 |
| Piezas rechazadas | 39 |
| Scrap (%) | 2.60 |
| Conformidad (%) | 97.40 |
| Fuerza promedio (N) | 12509.19 |
| Tiempo promedio (s) | 23.49 |
| Displacement promedio (mm) | 173.21 |

---

## Beneficios esperados

- Reducción de scrap.
- Menor tiempo de ajuste de programas.
- Mayor estabilidad del proceso.
- Mejor aprovechamiento de información histórica.
- Soporte para producción de alto volumen.

---

## Autor

**Brayan Augusto Ramírez Pompa**

Proyecto Integrador de Tecnologías de Big Data
