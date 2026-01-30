# Order_Matrix: Normalización de Matriz de Contrato 130

Este repositorio contiene las herramientas y scripts desarrollados en **R** para la limpieza, transformación y ordenamiento de la **Matriz de Contrato 130 (VP Codelco)**. 

El objetivo principal es procesar los datos brutos provenientes de planillas Excel para llevarlos a su **Primera Forma Normal (1FN)**, sentando las bases para una migración exitosa hacia una base de datos relacional (SQL).

## Objetivo del Proyecto

Transformar la matriz técnica general (Excel) en un conjunto de datos estructurado que cumpla con:
1. **Atomicidad:** Cada celda contiene un solo valor.
2. **Eliminación de grupos repetidos:** Creación de registros únicos por fila.
3. **Identificación de claves:** Preparación de campos para llaves primarias y foráneas.

## 🛠Tecnologías Utilizadas

* **Lenguaje:** R
* **Librerías principales:** `tidyverse`, `readxl`, `dplyr`
* **Entorno:** RStudio / Posit

## Estructura del Repositorio

* `ordenar_matriz.R`: Script principal con la lógica de limpieza y ordenamiento.
* `.gitignore`: Configuración para excluir archivos temporales y planillas Excel locales con datos sensibles (Andes Norte / Matrix130).

## Instrucciones de Uso

1. Colocar el archivo `Matrix130.xlsx` o `Matriz técnica general Andes Norte REV.0.xlsx` en la raíz del proyecto (estos archivos están ignorados por Git por seguridad).
2. Ejecutar el script `ordenar_matriz.R`.
3. El script generará una salida procesada lista para ser importada a un motor de base de datos.

---
**Nota:** Este proyecto es parte de la fase de pre-procesamiento de datos para la gestión de mantenimiento e inventarios de ingeniería civil industrial.