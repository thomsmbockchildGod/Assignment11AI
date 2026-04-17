#project Overview Assignment11AI
This project overall aimed , based on images (inputs data) predicts output variables (category).
The pipeline of our project is :Data(Image)-preprocessing-model training-prediction-evaluation
#Data(Image): we used the import OS to access our dataset(Images) located in folders . OS, is acting like a middle helping nagivate trough our folder.
Once the dataset(images) have been accessed, we used the openCV librairy to read and process our image
img=cv2.imread(img_path) (read the image in matrix from ) & img=cv2.resize(img,(64,64)) & img=cv2.cvtColor(cv2,color_RGB2BGR)
To predict our output variable, we defined the input(X) and output (Y) variables.
For the preprocessing steps we've flattened and scaled the input (X) variable by using the X=X.reshape(X.shape[0],-1), and the standardScaler()
After we split the model into training and testing set.
For the model evaluation, two models were used Random Forest and SVC. we processed to train the models (model.fit(X_train, y_train)) and after training, we predicted (y_pred) based on the testing set (X_test).
For the evaluation we used confusion_matrix, classification report and accuracy to evaluate both models.

Running of notebook
- Google colab link was shared to access the code
- once clicking on the link, notebook containing the code will be availbale
- clicking on the running button will run each code on each cells 
