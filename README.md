An Artificial Intelligence and Cloud Based Collaborative Platform for Plant Disease Identification, Tracking and Forecasting for Farmers

In this project author using convolution neural networks as artificial intelligence to train all plant diseases images and then upon uploading new images CNN will predict plant disease available in uploaded image. For storing CNN train model and images author is using cloud services. So using AI author predicting plant disease and cloud is used to store data.

In this project author using smart phone to upload image but designing android application will take extra cost and time so we build it as PYTHON web application. Using this web application CNN model will get trained and user can upload images and then application will apply CNN model on uploaded image to predict disease. If this web application deployed on real web server then it will extract user’s location from request object and can display those locations in map. If you run in local machine then we will get default IP ‘127.0.0.1’ and for this IP will get only default latitude and longitude. 

To implement this project we are using plant disease images dataset from ‘PlantVillage’ web site.

Python Django Server act like a cloud and web server

MYSQL database: used to store user’s details and their uploaded images location details.

To run this project install python 3.7 and then install MYSQL database and create database in MYSQL by copying content from ‘DB.txt’ file and paste in MYSQL.

Install below packages by opening command prompt and executing below commands

Pip install django
Pip install pymysql
pip install geoip2

after installing above command put ‘PlantDisease’ folder in any directory of your system and then open command prompt and set location to PlantDisease and execute below command to start server

python manage.py runserver



after executing above command will get below server screen

In above screen python server started and running on IP http://127.0.0.1:8000’. Now open browser and enter URL as ‘http://127.0.0.1:8000/index.html’ to get below screen





In above screen click on ‘Register Here’ link to allow user to register with the application


In above screen click on ‘Register’ button to add new user


In above screen user signup process completed. Now user can click on ‘Login’ link to login to application


After login will get below screen


In above screen click on ‘Upload Plant Image’ link to get below screen


In above screen user can upload image of his crop to predict disease using CNN


In above screen uploading 1.JPG image and now click on ‘Open’ button to upload image


In above screen click on ‘Submit’ button to predict disease


In above screen we will get image with predicted disease name printed on image and now close that image to get locations in map


In above screen in map we can get location of uploaded image mark with marker and below map we can see predicted disease name in red colour. Similarly you can upload any image from ‘uploadimages’ folder. In below screen we can see CNN layers created to build plant disease model


In above screen we can see CNN multi layers filter created where first filter created with image size 62 X 62 and second filter with size 31 X 31 and goes on.
