## **Overview**

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

## **Results**

* Data Preprocessing
  * What variable(s) are the target(s) for your model?
    * The target variable for the model is IS_SUCCESSFUL.
  * What variable(s) are the features for your model?
    * The feature variables for the model are APPLICATION_TYPE and CLASSIFICATION
  * What variable(s) should be removed from the input data because they are neither targets nor features?
    * The variable that should be removed is EIN because it does not contribute to the model's predictive power.

* Compiling, Training, and Evaluating the Model
  * How many neurons, layers, and activation functions did you select for your neural network model, and why?
    * Number of neurons: The number of neurons in the first hidden layer is 225 (hidden_nodes_layer1) and there are 37 neurons in the second layer (hidden_nodes_layer2).
    * Number of layers:  The model has 2 hidden layers.
    * Activation functions: The activation function used the hidden layers is ReLU and sigmoid is used in the output layer.
    * Why? I began by using examples from course materials and duplicated the number of layers and neurons and the activation functions.
    * Initial Solution:

      ![image](https://github.com/lphelpspittman/Deep_Learning_Challenge/assets/127759770/2c97f7dc-8149-46f9-ac56-952f0db878ff)

    * Final Solution

      ![image](https://github.com/lphelpspittman/Deep_Learning_Challenge/assets/127759770/fe8ddeb1-9057-4753-a636-b37af24662bf)

  * Were you able to achieve the target model performance?
    * The first model produced an accuracy rate of 72%.

      ![image](https://github.com/lphelpspittman/Deep_Learning_Challenge/assets/127759770/3cff8001-c417-4ce9-8c45-c44f2cb20bd1)

    * My final model produced an accuracy rate of just over 75%

      ![image](https://github.com/lphelpspittman/Deep_Learning_Challenge/assets/127759770/fbafffc9-8874-4701-87fe-c9b6b98357cc)

  * What steps did you take in your attempts to increase model performance?
    * I added a third hidden layer, but that did not increase my accuracy enough.  I added the NAME column back to the model and boosted the accuracy rate to over 75%.

## **Summary**

This deep learning model, a neural network, was designed to reach the required accuracy rate for determining successful funding by Alphabet Soup.  This model can be recommended because it fulfills the requirement of achieving over 75% accuracy in its predictions, however I believe using a different approach, such as Random Forest, could produce better results.
