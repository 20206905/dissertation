# Dissertation
The implementation for my dissertation "Predicting the Weight of a Human from a Photo".

# How to run
1) Load up the "new" folder into VS Code.
2) Open the built-in Terminal and run "nodemon app.js".
3) In Google Chrome navigate to "localhost:3000".

The above is the data collection method, it goes through the images in the "archive" folder, estimates the body pose & segmentation and then the anthropometric features. After this is done for each photo the anthropometric feature ratios along with the weight of the subject are added to a data array as an object, and at the end a JSON file is installed onto the compute using the neuralNetwork library.

4) Next, load up the "neural_network" folder into VS Code.
5) Open the built-in Terminal and run "nodemon app.js".
6) In Google Chrom navigate to "localhost:3000".

In the above the "anthropometricFeatures.json" file created in the "new" folder is loaded into the "sketch.js" file into an array called "data". A testing dataset is then taken from this at random, then the model is trained and tested. The results of the tests are in the Console alonog with the Mean Absolute Error and Mean Absolute Percentage Error.
