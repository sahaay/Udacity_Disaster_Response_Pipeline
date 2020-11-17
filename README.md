## Disaster Response Pipeline

This project is to analyze disaster data from [Figure Eight](www.figure-eight.com) to build a model for an API that classifies disaster messages.

### Project Folders

* Data
  * **process_data.py** : reads in the data, cleans and stores it in a SQL database
  * **disaster_categories.csv** and **disaster_messages.csv** : datasets provided
  * **DisasterResponse.db** : database created by transformed and cleaned data
  
* Models
  * **train_classifier.py** : code to load data, transform it using natural language processing, run a machine learning model using GridSearchCV and train it
  
* App
  * **run.py** : Flask app and the user interface used to predict and display the results
  * **templates** : folder containing the HTML templates for the output
  
### Example code 

python process_data.py disaster_messages.csv disaster_categories.csv DisasterResponse.db

python train_classifier.py ../data/DisasterResponse.db classifier.pkl

python run.py

### Screenshots from the app

Screenshot 1

![Screenshot 1](https://user-images.githubusercontent.com/36114952/99365486-45c72900-28af-11eb-8677-04823816f4a3.png)

Screenshot 2

![Screenshot 2](https://user-images.githubusercontent.com/36114952/99365721-93439600-28af-11eb-860d-6e72fffbf307.png)


### Acknowledgements

Data provided by [Figure Eight](www.figure-eight.com) and this project is done as part of Data Science Nanodegree by [Udacity](www.udacity.com).
