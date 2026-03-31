# Smart_Recipe_Recommender

**Overview : **
This project is a Flask-based web application that combines computer vision and API integration to provide a smart cooking assistant.
The system allows users to upload an image of food items, automatically detects ingredients using a YOLOv10 object detection model, and then fetches relevant recipes using the Spoonacular API.

It is especially useful for:
1. Reducing food waste .
2. Discovering recipes with available ingredients.
3. Helping beginners cook easily.

Objectives:
1. Automate ingredient detection from images.
2. Provide real-time recipe suggestions.
3. Reduce manual effort in searching recipes.
4. Demonstrate integration of AI with web development.

**Features provided by this project:**
1. Image Upload: Users can upload food images.
2.  Object Detection: Detects ingredients using YOLO model.
3.  Ingredient Filtering: Only relevant food classes are considered.
4.  Recipe Suggestions: Fetches recipes based on detected ingredients.
5.  Direct Links: Provides clickable recipe URLs.
6.   Fast API Response: Efficient backend processing.

**Tech Stack**
  -- Backend
Flask (Python web framework)
Flask-CORS (for handling cross-origin requests)
  -- AI / ML
YOLOv10 (Ultralytics) for object detection
  -- API Integration
Spoonacular API for recipe data
  -- Libraries Used
ultralytics – for YOLO model
Pillow – for image processing
requests – for API calls
io, os – file handling

**Working Principle**

Step 1: Image Upload

User uploads an image via the web interface.

Step 2: Image Processing
Image is converted to RGB format
Temporarily saved and passed to YOLO model
Step 3: Object Detection
Model detects objects in the image
Filters only predefined food items:
apple, banana, orange, broccoli, carrot
Step 4: Recipe Fetching
Detected ingredients are sent to Spoonacular API
API returns matching recipes
Step 5: Output Display

User gets:

Detected ingredients
Recipes list
Missing ingredients
Recipe links
