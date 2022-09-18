# MNIST-Using-Jupyter-Notebook
Classification of MNIST dataset using Jupyter Notebook. There are two two types of neural network used,
- A model with One with Input layer and Ouptput Layer and,
´´´  
model = keras.Sequential([keras.layers.Flatten(input_shape=(28, 28)),
                        keras.layers.Dense(10, activation='sigmoid')
                        ])
model.compile(optimizer='adam',
              loss='sparse_categorical_crossentropy',
              metrics=['accuracy']
             )
model.fit(X_train, y_train, epochs=5)
´´´
- Other with one additional layer i.e. Hidden Layer
The code check the performance of the model and is an attempt to check the influence of hidden layer on datasets.

# Experiments
The expermiment performed is based on the confusion matrix as follows,

<table>
  <tr>
    <td>Without Hidden layer</td>
     <td>With Hidden layer</td>
  </tr>
  <tr>
    <td><img src="https://github.com/amitk0693/MNIST-Using-Jupyter-Notebook/blob/55f81e1b546569a37d71110c34cd5f5ed022c9c8/cnf1.png" width=380 height=280></td>
    <td><img src="https://github.com/amitk0693/MNIST-Using-Jupyter-Notebook/blob/55f81e1b546569a37d71110c34cd5f5ed022c9c8/cnf2.png" width=380 height=280></td>
  </tr>
 </table>
 
The performance of Deep Learning Network is better with hidden units.
