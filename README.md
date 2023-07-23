# Recipe-Recommendation-System

## Working:
1. There exists a normal search bar which allows you to search for recipes based on the ingredients or the recipes as such.
2. If you require personal recommendations, you switch over to Recommendation section where you'll find a button called 'Display Current Stock'.
3. On clicking that button, a request is sent to an endpoint which in turn returns the base64-encoded image from the ESP32 CAM powered by Arduino WebServer.
4. The image gets displayed in the website and another button called 'Predict Current Stock' pops up.
5. On clicking that button, a POST request is sent to another endpoint which in turn processes the image through InceptionV3 Model (Machine Learning) powered by FastAPI and returns the predicted ingredient.
6. The ingredient name gets displayed and another form pops up which takes your preferntial input like gluten, dairy, veg, etc.
7. On submitting that form, you'll be taken to the 'Fetch Recommendations' section where on clicking the button, a GET request will be sent to the Spoonacular API that fetches all the recipes along its information.

## Tech Stack
1. Website -> React JS, Tailwindcss, Firebase
2. Hardware -> Arduino IDE
3. ML Model -> Python, FastAPI, Tensorflow
