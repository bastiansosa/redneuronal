
Este proyecto aborda el problema de limpiar imágenes de texto afectadas por ruido mediante el uso de Autoencoders.

Se utilizan dos bases de datos principales:

train_clean: contiene imágenes de texto escrito sin ruido ni contaminación visual.

train_noise: contiene las mismas imágenes, pero con distintos niveles de ruido que dificultan la lectura.

El modelo propuesto es un Autoencoder convolucional que aprende a reconstruir imágenes limpias a partir de ejemplos sin ruido. Una vez entrenado, este modelo es capaz de recibir como entrada una imagen con ruido y generar como salida una versión descontaminada y más legible.

En resumen, el flujo de trabajo es:

Entrenar el autoencoder usando las imágenes limpias (train_clean) como referencia.

Alimentar el modelo con imágenes ruidosas (train_noise).

Obtener como resultado imágenes denoised, donde el texto se presenta de forma clara y legible.

Este enfoque puede aplicarse en preprocesamiento de OCR, digitalización de documentos antiguos, mejora de datasets con imágenes contaminadas y otras aplicaciones donde la calidad del texto visual es crítica.
