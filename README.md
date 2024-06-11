# Project Short Note

The challenge is to classify histopathologic images into cancerous and non-cancerous categories using a CNN. The dataset consists of thousands of RGB images, each resized to 128x128 pixels, organized into training and test directories. This task involves image preprocessing, data augmentation, and model training using deep learning techniques.


### Result of Hyper-Parameter Tuning

I experimented with Different Optimizers, Learning Rates and Dropout Rates.  Here are teh summary


| Hyperparameter | Value | Train Accuracy | Validation Accuracy |
|----------------|-------|----------------|---------------------|
| Optimizer      | Adam  | 0.786148       | 0.803672            |
| Optimizer      | RMSprop | 0.773559     | 0.805085            |
| Optimizer      | SGD   | 0.793661       | 0.788047            |
| Learning Rate  | 0.001 | 0.817198       | 0.825653            |
| Learning Rate  | 0.0001 | 0.818129      | 0.820180            |
| Learning Rate  | 0.01  | 0.595146       | 0.592161            |
| Dropout Rate   | 0.3   | 0.822584       | 0.777013            |
| Dropout Rate   | 0.5   | 0.809100       | 0.816649            |
| Dropout Rate   | 0.7   | 0.762744       | 0.794315            |


### Description of the Result

The table above presents the results of hyperparameter tuning for a machine learning model, showcasing the train and validation accuracy for various configurations. Here is a summary of the key findings:

- **Best Optimizer**: RMSprop with a validation accuracy of 0.805085.
- **Best Learning Rate**: 0.001 with the highest validation accuracy of 0.825653.
- **Best Dropout Rate**: 0.5 with a balanced train accuracy of 0.809100 and validation accuracy of 0.816649.

The optimal configuration appears to be using RMSprop optimizer with a learning rate of 0.001 and a dropout rate of 0.5 for achieving the best balance between training and validation performance.