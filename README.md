**Create the SMS Classification Function**  
Using the code in the sms_text_classification_solution.ipynb file, create the sms_classification function in the gradio_sms_text_classification.ipynb by doing the following:  

Set the features variable to the text message column of the DataFrame.  

Set the target variable to the "label" column of the DataFrame.  

Split data into training and testing and set the test_size to 33%.  

Build a pipeline to transform the test set to compare to the training set.  

Fit the model to the transformed training data and return model.  

Load the SMSSpamCollection.csv into a DataFrame and call the sms_classification function with the DataFrame, and set the result to the "text_clf" variable.  

**Create the SMS Prediction Function**  
Use the sms_prediction function to predict the classification of a new text by doing the following:  

Create a variable that will hold the prediction of a new text.  

Use a conditional statement that determines if the text message is "ham" or “spam”.  

If the message is “ham”, the function should return the following message: f'The text message: "{text}", is not spam.'  

If the message is spam, the function should return the following message: f'The text message: "{text}", is spam.'  

**Create the Gradio Interface Application**  
Create a Gradio Interface application that takes a textbox for the inputs and has a textbox for the output. The textboxes should have labels that describe what each textbox contains.  

Launch the application and provide the URL to share the application. Your application should look like the following:  

The SMS prediction Gradio application interface  
Use the following text messages to test your application.  

1. You are a lucky winner of $5000!  
2. You won 2 free tickets to the Super Bowl.  
3. You won 2 free tickets to the Super Bowl. Text us to claim your prize.  
4. Thanks for registering. Text 4343 to receive free updates on medicare.  

**Requirements**  
Create the SMS Classification Function  
The features variable is set equal to the text message column of the DataFrame.  

The target variable is set equal to the "label" column of the DataFrame. 

The data is split into training and testing sets, and the test_size is set to 33%. 

A Pipeline is built using the TfidfVectorizer and LinearSVC to transform the test set and compare it to the training set. 

The model is fitted to the transformed training data and the model is returned. 

The SMSSpamCollection.csv is read into a DataFrame. 

The DataFrame is passed to the sms_classification function and the result is set equal to the "text_clf" variable. 

**Create the SMS Prediction Function **  
A variable that holds the prediction of a new text is created.  

A conditional statement that determines if the text message is "ham" or “spam” is created. 

The conditional returns a message if the text is “ham”. 

The conditional returns a message if the text is “spam”. 

**Create the Gradio Interface Application **  
A Gradio Interface application is created with three parameters for the “function”, “outputs”, and “inputs”. 

The “outputs” parameter is a textbox that contains a label to let the user know what to type in the box.  

The “inputs” parameter is a textbox that contains a label to let the user know that the prediction will be displayed in the textbox. 

The Interface application can be shared with other users with a public URL.  

The Gradio Interface works as expected and there are no errors after a user submits a text message.  