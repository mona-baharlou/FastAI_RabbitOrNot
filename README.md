## Is it a Rabbit?
This repository contains a simple, yet powerful, image classification model built using the fastai library. The model is trained to distinguish between images of rabbits and images of houses. This project serves as a foundational example of a complete end-to-end deep learning pipeline, from data acquisition and preparation to model training and prediction.

This project was developed as a practical exercise while following the Practical Deep Learning for Coders course by Jeremy Howard. It's a great example of how to leverage transfer learning and high-level libraries like fastai to build a robust classifier with minimal code.

# How It Works
 - Data Acquisition: Images for both 'rabbit' and 'house' classes are automatically downloaded from the web using the duckduckgo_search library.
 - Data Cleaning: The downloaded images are verified for integrity, and any corrupted files are automatically removed.
 - Data Preparation: The images are organized and prepared for training using fastai's DataBlock API, which handles resizing, splitting the dataset into training and validation sets, and labeling.
 - Model Training: A pre-trained ResNet18 model is used for transfer learning, significantly reducing training time and improving accuracy. The model is fine-tuned on the new dataset.
 - Prediction: The trained model can then be used to predict whether a new, unseen image is a rabbit or a house, along with a confidence score.

# Technologies Used
 - fastai: The deep learning library used to build and train the model.
 - duckduckgo_search: Used for scraping image URLs from the web.
 - pathlib: For handling file system paths in a modern, object-oriented way.
 - Pillow (PIL): For image manipulation and display.

# Example Output
After training, the model can make a prediction on a new image. A typical output would look like this:

> This is a: rabbit.
> Probability it's a rabbit: 0.9987

![](https://github.com/mona-baharlou/FastAI_RabbitOrNot/blob/main/RabbitOrHouse.png)
