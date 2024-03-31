# sms_spam_detector
## The Challenge
>You'll be refactoring code from an SMS text classification solution into a
>function that constructs a linear Support Vector Classification (SVC) model.
>Once the model is created and trained, you will create a Gradio app to host the
>application, enabling users to test text messages. The application will provide
>feedback to users, indicating whether the text is classified as spam or not,
>based on the model's performance.
>
>
>## Files
>Download the following files to help you get started: Module 21 Challenge files
>(https://static.bc-edx.com/ai/ail-v-1-0/m21/lms/starter/M21_Starter_Code.zip)
>
>
## Getting Started
>Before starting the Challenge, be sure to complete the following steps:
>-  Create a new repository for this project called sms_spam_detector.
>   Do not add this homework assignment to an existing repository.
>-  Clone the new repository to your computer.
>-  Inside your local Git repository, add the starter files from your file
>downloads.
>-  Push these changes to GitHub or GitLab.
>
>
>## Instructions
>The starter files consist of the following files: 
>gradio_sms_text_classification.ipynb, sms_text_classification_solution.ipynb,
>and SMSSpamCollection.csv.
>
>### Create the SMS Classification Function
>1. Using the code in the sms_text_classification_solution.ipynb file, create
>the sms_classification function in the gradio_sms_text_classification.ipynb
>by doing the following:
>
>-  Set the features variable to the text message column of the DataFrame.
>
>-  Set the target variable to the "label" column of the DataFrame.
>
>-  Split data into training and testing and set the test_size to 33%.
>
>-  Build a pipeline to transform the test set to compare to the training set.
>
>-  Fit the model to the transformed training data and return model.
>
>2. Load the SMSSpamCollection.csv into a DataFrame and call the
>sms_classification function with the DataFrame, and set the result to the
>"text_clf" variable.
>
>### Create the SMS Prediction Function
>Use the sms_prediction function to predict the classification of a new text by
>doing the following:
>
>-  Use a conditional statement that determines if the text message is "ham" or
>   “spam”.
>
>-- If the message is “ham”, the function should return the following message:
>   f'The text message: "{text}", is not spam.'
>
>-- If the message is spam, the function should return the following message:
>   f'The text message: "{text}", is spam.'
>
>
>### Create the Gradio Interface Application
>1. Create a Gradio Interface application that takes a textbox for the inputs
>and has a textbox for the output. The textboxes should have labels that
>describe what each textbox contains.
>
>2. Launch the application and provide the URL to share the application. Your
>application should look like the following:
>
>![mod-21-ref-image](https://github.com/RAC-Git-Hub/sms_spam_detector/blob/main/Resources/mod-21-ref-image.png)
>
>
>3. Use the following text messages to test your aplication.
>
>![mod-21-ref-image-2](https://github.com/RAC-Git-Hub/sms_spam_detector/blob/main/Resources/mod-21-ref-image-2.png)
>
>
## Sources
The starter codes were obtained in March 2024 from the instructional staff of
the OSU AI Bootcamp and were generated by edX Boot Camps LLC.
## Collaborators
Although this project was done individually, the skillset used to complete this 
assignment is a culmination of knowledge learned in the classroom setting which
includes lecture materials, example programming from instructors, interactive
dialogue in group settings among fellow students, independent internet research,
and some general programming guidance from sources such as CoPilot and ChatGPT. 