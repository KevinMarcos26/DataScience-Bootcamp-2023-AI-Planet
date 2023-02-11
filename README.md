# DataScience-Bootcamp-2023-AI-Planet
Ai Planet Bootcam 5 Weeks Data Science

Desafío AI/ML

Un hospital en la provincia de Groenlandia ha estado tratando de mejorar sus condiciones de atención al observar la supervivencia histórica de los pacientes. Intentaron mirar sus datos, pero no pudieron identificar los principales factores que conducen a altas supervivencias.

Objetivo
Eres el mejor científico de datos en Groenlandia y te han contratado para resolver este problema. Ahora usted es responsable de desarrollar un modelo que prediga las posibilidades de supervivencia de un paciente después de 1 año de tratamiento (Survived_1_year).

Criterios de evaluación
Las presentaciones se evalúan utilizando el puntaje F1. ¿Cómo lo hacemos?

Una vez que genere y envíe las predicciones de la variable objetivo en el conjunto de datos de evaluación, sus envíos se compararán con los valores reales de la variable objetivo.

Los valores True o Actual de la variable objetivo están ocultos en la plataforma DPhi Practice para que podamos evaluar el rendimiento de su modelo en los datos de evaluación. Finalmente, se generará y mostrará una puntuación F1 para su modelo.

Acerca del conjunto de datos
El conjunto de datos contiene los registros de pacientes recopilados de un hospital en Groenlandia. La columna "Survived_1_year" es una variable de destino que tiene entradas binarias (0 o 1).

Survived_1_year == 0, implica que el paciente no sobrevivió después de 1 año de tratamiento

Survived_1_year == 1, implica que el paciente sobrevivió después de 1 año de tratamiento

Para cargar el conjunto de datos en Jupyter Notebook, use el siguiente comando:

import pandas as pd
pharma_data = pd.read_csv('https://raw.githubusercontent.com/dphi-official/Datasets/master/pharma_data/Training_set_begs.csv')

Descripción de los datos:

ID_Patient_Care_Situation: Situación asistencial de un paciente durante el tratamiento

Diagnosed_Condition: La condición diagnosticada del paciente

ID_Patient: Número de identificación del paciente

Treatment_with_drugs: Clase de medicamentos utilizados durante el tratamiento

Survived_1_year: Si el paciente sobrevivió después de un año (0 significa que no sobrevivió; 1 significa que sobrevivió)

Patient_Age: Edad del paciente

Patient_Body_Mass_Index: Un valor calculado basado en el peso, altura, etc. del paciente.

Patient_Smoker: Si el paciente era fumador o no

Patient_Rural_Urban: Si el paciente se quedó en la zona rural o urbana del país

Previous_Condition: Condición del paciente antes del inicio del tratamiento ( Esta variable se divide en 8 columnas: A, B, C, D, E, F, Z y Number_of_prev_cond. A, B, C, D, E, F y Z son las condiciones previas del paciente. Supongamos que para un paciente, si la entrada en la columna A es 1, significa que la condición previa del paciente era A. Si el paciente no tenía esa condición, es 0 y lo mismo para otras condiciones. Si un paciente tiene una condición previa como A y C, las columnas A y C tendrán entradas como 1 y 1 respectivamente, mientras que la otra columna B, D, E, F, Z tendrá entradas 0, 0, 0, 0, 0 respectivamente. La columna Number_of_prev_cond tendrá la entrada como 2, es decir, 1 + 0 + 1 + 0 + 0 + 0 + 0 + 0 = 2 en este caso. )

Siéntase libre de buscar en Google 'Diagnosticar' e 'Índice de masa corporal' si no conoce estos términos.

Para cargar el conjunto de datos de prueba en Jupyter Notebook, use el siguiente comando:


test_data = pd.read_csv('https://raw.githubusercontent.com/dphi-official/Datasets/master/pharma_data/Testing_set_begs.csv')
Recursos
Datos del tren

Datos de prueba

Envío de muestras

Directrices para la presentación
1. Su archivo de predicciones debe ser un CSV y su primera fila, es decir, el campo de encabezado debe ser predicción

2. Debe cargar el archivo de bloc de notas .ipynb como solución a la pregunta

Métrica de evaluación
La métrica de evaluación F1Score se utiliza para evaluar las predicciones del modelo

Directrices adicionales
Puede realizar cualquier número de envíos.

Asegúrese de enviar tanto el archivo de predicción como el bloc de notas antes de la fecha de finalización

Prueba
