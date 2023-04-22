# ML_bootcamp

# Ejercicio Machine Learning del Bootcamp de TheBridge Data Science
 
Como ejercicio de aprendizaje de los contenidos vistos sobre Machine Learning en el Bootcamp de The Bridge, realizo un proyecto con datos obtenidos de Kaggle para su estudio y testeo con un sistema predictivo de clasificación.


## Projects:

###  Does it shine bright like a diamond?

El objetivo (inventado) del proyecto es estudiar los datos obtenidos del dataset de Kaggle. Valorar sus columnas, correlaciones y decidir desde un punto de vista técnico-estadístico cuales son las variables que nos pueda ayudar a predecir la necesidad demandada desde negocio. A esas variables añadirles las relevantes para el área de negocio.
Como algunas variables son "object" las convertiremos a tipo "numeric" con el método de preprocessing LabelEnconder. Así estas variables estarán a disposición de los métodos predictivos si fuera necesario usarlas.
Para determinar las columnas más relevantes utilzaré un random forest classifier y el método feature_importances_
![image](https://github.com/jorgeirish/ML_bootcamp/blob/550220057e34389fde32dd9ac73e20cdf39d5670/feature_importances_.JPG?raw=true])

---
 
### Algunos datos relavantes del EDA
 
 Para valorar las importancias y relaciones (en nuestro caso las correlaciones entre columnas) es importante realizar un pairplot donde se aprecie la ubicación de nuestros datos respecto a esos ejes. En la carpeta hay diferentes gráficos relevantes.
 Comparto (para destacar) una imagen del estudio con los puntos pintados por el target del estudio: el corte.
 ![image](https://github.com/jorgeirish/ML_bootcamp/blob/66b07a0c352f5e72225ba67e8b08ca9cca469963/pairplot.png?raw=true])
 
---
 
### Modelos de Machine Learning

Dos modelos de machine learning propuestos en el desarrollo de este trabajo.
* Random Forest Classifier
* AdaBoost Classifier

Para encontrar el mejor scoring nos ayudamos de un GridSearchCV con diferentes variables. El objetivo es con los datos obtener el mejor % de precesión para predecir el tipo de corte que tendrá el diamante y valorar así como de brillante es dicho diamante.

---

### Créditos y autoria

Los datos han sido obtenidos de Kaggle (https://www.kaggle.com/datasets/shivam2503/diamonds)
Herramientas y guía de mis profesores de bootcamp de TheBridge: Alberto, John y Alejandro
Código e idea propias, Jorge Fernández
