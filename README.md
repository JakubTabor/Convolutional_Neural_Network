# Convolutional_Neural_Network
# First I need to preprocess my images, so I "rescale" them, then create some samples in different  configurations np. " zoom_range = 0.2, horizontal_flip" 
# Then i need to specify my dataset and parameters, so I set "target_size to be (64, 64), batch_size to be 32, class_mode is binary"
# Next from directory I choose "training_set" I do exactly the same preprocess with my "test_set"
# Now when I have my sets ready for training I create "cnn model" "tf.keras.models.Sequential()"
# Then I create first convolutional 2D layer that will have "32 filters" this number its just a try, my kernel size will be (3) and activation "relu"
# "input_shape" will be "[64, 64, 3]", then I add pool layer which size will be (2, 2) "pool_size=2, strides=2"
# Next I add hidden layer with this same parameters as my first layer and then pool layer with size (2, 2)
# Thats all my convolutional layers, now i need to "flatten" them, because they need to fit to my whole network, so i add "Flatten layer"
# Now I add additional "Dense layer" with (128 neurons and activation relu" and "output layer" with "one neuron" and "activation sigmoid"
# Then I need to compile my model with "optimizer adam", "loss will be binary_crossentropy" because i have binary output and "metrics will be accuracy" 
# Finally I train my model with "x as training_set and validation_data as test_set" and "25 epochs"
