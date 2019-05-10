# Malaria_cell_detector.
Comparison between a CNN and a VGG16 for the diagnosis of malaria.Using Keras
# Informe
Esta práctica se ha basado en el siguiente dataset:
https://www.kaggle.com/iarunava/cell-images-for-detecting-malaria
Se trata de identificar entre células infectadas malaria y sanas, más concretamente glóbulos rojos.Para ello se compara los resultados de un red basada en la VGG16 y una CNN adaptada al problema.
Para llegar a resultados decentes se ha sustituido la capa densa y se ha recalculado los pesos de algunas capas convolutivas intermedias.Debido a que la VGG16 con los pesos del dataset imagenet no son pesos adecuados para poder identificar la zona infectada de los glóbulos. Se llega aproximadamente a un 94% de accuracy y validation.
Se introduce varias capas de maxpooling para poder caracterizar las zonas y patrones más característicos de las imágenes.Asimismo se introduce varias capas dropout para reducir el posible sobreajuste. Se llega a un 92% de acurracy y validation.
