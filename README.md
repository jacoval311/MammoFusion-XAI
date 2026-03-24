# MammoFusion-XAI 🎗️💻

### Integración Multimodal para el Soporte al Diagnóstico de Cáncer de Mama

Este proyecto implementa un modelo de **Aprendizaje Profundo Multimodal** que combina el análisis de visión por computadora de mamografías con datos tabulares de biomarcadores clínicos. El objetivo es reducir los falsos positivos en el tamizaje y proporcionar herramientas explicables a los radiólogos.

## 1. Arquitectura del Modelo
El sistema utiliza una arquitectura de **Fusión Intermedia (Mid-fusion)**:
- **Rama de Imagen:** CNN (EfficientNetV2 o ResNet50) para extraer características espaciales de las mamografías.
- **Rama Tabular:** MLP (Multilayer Perceptron) para procesar edad y biomarcadores (HER2, ER, PR, Ki-67).
- **Concatenación:** Un vector conjunto alimenta las capas densas finales para la clasificación.

## 2. Dataset
Se utilizan subconjuntos curados de:
- **CBIS-DDSM:** Para imágenes y etiquetas de patología.
- **TCGA-BRCA / METABRIC:** Para la lógica de correlación con biomarcadores moleculares.

## 3. Instalación
```bash
git clone [https://github.com/tu-usuario/MammoFusion-XAI.git](https://github.com/tu-usuario/MammoFusion-XAI.git)
pip install -r requirements.txt
