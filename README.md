# Convolutional_Neural_Network
# First I need to preprocess my images, so I "rescale" them, then create some samples in different  configurations np. " zoom_range = 0.2, horizontal_flip" 
# Then i need to specify my dataset and parameters, so I set "target_size to be (64, 64), batch_size to be 32, class_mode is binary"
# Next from directory I choose "training_set" I do exactly the same preprocess with my "test_set"
# Now when I have my sets ready for training I create "cnn model" "tf.keras.models.Sequential()"
# Then I create first convolutional 2D layer that will have "32 filters" this number its just a try, my kernel size will be (3) and activation "relu"
