# OBJECTIVE: Install MongoDB database and use it for Sentiment analysis project in the current GitHub repository.
Fot technical reasons, I put MongoDB part in the [Sentiment Analysis project](https://github.com/PavelPll/Sentiment_ETL_Analysis) of the current GitHub. The file, docker-compose.yml, run the container c1, with installed Python (Jupyter notebook) and two MongoDB containers. 
* The first container, c1, is used to run the code.
* The second container, **my_mongo**, is used to store the data (use my_mongo:27017 to access stored data from Python and Jupyter notebook).
* The third one, **mongo-express**, is used for MongoDB Graphic User Interface (http://localhost:8081).
