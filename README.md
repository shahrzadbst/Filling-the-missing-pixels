# Filling-the-missing-pixels
Filling the missing pixels in an image using factor graphs and Sum-Product algorithms

This project was developed as part of a direct studies course on Pattern Recognition and Machine Learning. Our objective was to utilize the MNIST image dataset and explore the task of removing a randomly selected square within the images. Subsequently, we aimed to fill the missing pixels by determining their correct values using factor graphs and the Sum-Product algorithm.

The MNIST dataset is widely recognized in the field of machine learning and comprises handwritten digits ranging from 0 to 9. Each digit image is represented as a grayscale pixel matrix with dimensions of 28x28.

Factor graphs serve as graphical models that facilitate the decomposition of joint probability distributions into smaller factors. They offer an effective means of expressing intricate probabilistic relationships between variables in a concise and comprehensible manner.

The Sum-Product algorithm, also referred to as the belief propagation algorithm, is an efficient method employed for computing marginal probabilities within graphical models. Specifically designed to operate on factor graphs, this algorithm employs iterative message updates between nodes to propagate information and compute beliefs about the variables.

In our project, we represented each pixel in the MNIST images as a variable within the factor graph. Initially, the variables corresponding to the removed square were observed as missing, and we assigned them uniform or prior probabilities.

By employing the Sum-Product algorithm, we performed iterative updates of messages between the variables and factors in the factor graph. This allowed us to estimate the probabilities of the missing pixels by leveraging the information carried by the observed pixels and their relationships with the missing pixels. Consequently, we were able to infer the most likely values for the missing pixels and accurately reconstruct the complete digit images.

Throughout our analysis, we evaluated and examined the outcomes of our approach by comparing them against the ground truth values in the original MNIST dataset. This process enabled us to assess the efficacy and accuracy of our method in successfully filling in the missing pixel values and reconstructing the complete digit images.
