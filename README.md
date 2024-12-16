create a Python-based API using Flask or Django. • The API should include the following endpoints:</br>
1. POST /add-app: Add app details to the database (fields: app_name, version, description).</br>
2. GET /get-app/{id}: Retrieve app details by ID.</br>
3. DELETE /delete-app/{id}: Remove an app by ID</br>
Step 1: Set Up Your Django Project.</br>
Install Django and Django REST framework</br>
Create a Django Project</br>
Add the App to INSTALLED_APPS</br>
Step 2: Define Your Models</br>
Step 3: Create Serializers</br>
Step 4: Create Views</br>
Step 5: Define URLs</br>
Step 6: Run Migrations and Start the Server</br>
2. Design a simple SQLite or PostgreSQL database to store app information (app_name, version, description).</br>
Step 1: Define the Database Model</br>
Step 2: Configure the Database</br>
Step 3: Run Migrations</br>
Step 4: Update API Views - class ApplicationCreate, class ApplicationDetail</br>
Step 5: Define URLs – api/add-app/ , api/get-app/<int:pk>/,api/delete-app/<int:pk>/</br>
Step 6: Start the Server – </br>
1.	python manage.py makemigrations</br>
2.	python manage.py migrate </br>
3.	Python manag.py runserver</br>
Example of output:</br>
	GET /api/get-app/1/
HTTP 200 OK
Allow: GET, DELETE, HEAD, OPTIONS
Content-Type: application/json
Vary: Accept

{
    "id": 1,
    "app_name": "rawData",
    "version": "2.0.2",
    "description": "new dec"
}

