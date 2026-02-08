# Fashion-MNIST-Image_Classification
https://colab.research.google.com/drive/1B9ycGgdSgvyW5KMLSYG6QMPoU19RzJ8y#scrollTo=wH6jI6ZwuG2p

1. What is the Fashion MNIST dataset?

The **Fashion MNIST dataset** consists of **70,000 grayscale images** of fashion products, each with a resolution of **28×28 pixels**.
It includes **10 categories of clothing items**, such as shirts, pants, footwear, and accessories.
This dataset is widely used for **training and evaluating machine learning models** and serves as a more complex alternative to the original MNIST handwritten digits dataset.

2. Why are image pixel values normalized before training?

Pixel normalization converts values from the **0–255 range to a 0–1 range.
This scaling allows neural networks to **learn more efficiently and converge faster**.
It also enhances **training stability and overall model performance**.

3. What layers are used in the neural network and what do they do?**

Flatten layer
  Transforms the 28×28 image into a single-dimensional vector so it can be fed into fully connected layers.

Dense layer (128 neurons with ReLU activation)
  Extracts meaningful patterns from the input data and adds non-linearity for better learning.

Dense output layer (10 neurons)
  Generates prediction scores for each of the 10 clothing categories.

4. What is an epoch in model training?

An **epoch** refers to **one full cycle through the entire training dataset**.
During each epoch, the model updates its parameters to improve accuracy.
Using multiple epochs helps the model **better recognize underlying patterns**.

5. How do the predicted and actual labels compare for the first test image?

The **predicted label** is the category selected by the model with the highest confidence score.
The **actual label** is the true category provided in the dataset.
When both labels are the same, the prediction is **correct**; otherwise, it is a **classification error**.

6. How can the model’s accuracy be improved?

* Train the model for **more epochs**
* Increase the **number of neurons or hidden layers**
* Introduce **Dropout layers** to prevent overfitting
* Use **data augmentation techniques**
* Adjust hyperparameters like **learning rate or batch size**
* Replace dense layers with a **Convolutional Neural Network (CNN)** for better image feature extraction
