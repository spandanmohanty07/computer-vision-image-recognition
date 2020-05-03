Objective - Classify whether an image is of a horse or a human (Binary Classification)
Environment used - Google colab GPU runtime

Download image training dataset - https://storage.googleapis.com/laurencemoroney-blog.appspot.com/horse-or-human.zip \
    -O /tmp/horse-or-human.zip
Download image validation dataset - https://storage.googleapis.com/laurencemoroney-blog.appspot.com/validation-horse-or-human.zip \
    -O /tmp/validation-horse-or-human.zip

Architecture - Sequential model with 5 convoltions layers are used
Optimizer function - RMSProp / Adam used. Both performed well.
Loss function - binary_crossentropy (since binary classification problem)

Image preprocessor - ImageDataGenerator is used. It will help in rescaling all the images in the specified directory. We don't have to label training and testing images. The name of the directory 'Human' or 'Horse' defines the label of a particular image.