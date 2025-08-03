# Detección de Apnea del Sueño mediante Modelos de Aprendizaje Profundo

Este repositorio contiene el notebook `SAOSdetector.ipynb`, desarrollado como parte de mi Proyecto Final de Grado en Bioingeniería. El objetivo principal es apoyar la detección de eventos de apnea e hipopnea a partir de la señal de saturación de oxígeno (SpO₂), utilizando modelos de aprendizaje profundo.

## Descripción del proyecto

La polisomnografía (PSG) es actualmente el estándar de referencia para el diagnóstico del Síndrome de Apnea Obstructiva del Sueño (SAOS), pero su uso está limitado por el alto costo, la necesidad de infraestructura especializada y su naturaleza intrusiva. Este trabajo propone un método alternativo y no invasivo basado únicamente en señales de oximetría de pulso, lo cual permite su implementación domiciliaria.

Mediante la optimización de un límite inferior de evidencia (ELBO), se estima la probabilidad de eventos respiratorios en función del comportamiento de la SpO₂. Para ello, se entrenó un modelo basado en arquitecturas de autoencoders variacionales (VAE) y redes generativas adversarias (GAN).

## Estructura del repositorio

- `SAOSdetector.ipynb`: notebook principal con la implementación del modelo y su evaluación.

## Dataset utilizado

Se utilizó la base de datos **Sleep Heart Health Study (SHHS)**, disponible públicamente para fines de investigación. Esta contiene registros polisomnográficos de adultos, incluyendo la señal de SpO₂ anotada con eventos respiratorios.

## Requisitos

Este proyecto fue desarrollado en Python 3.8. Las principales bibliotecas requeridas son:

- `numpy`
- `pandas`
- `matplotlib`
- `tensorflow` o `keras`
- `scikit-learn`
