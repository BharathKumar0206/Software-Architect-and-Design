# Hello World Django App

This is a simple Django web application that returns a JSON object with the message "Hello World!".

## Running the Application

To run the application locally, follow these steps:

1. Make sure you have Python and Django installed. If not, you can install Django using pip:

   ```
   pip install django
   ```

2. Clone this repository to your local machine:

   ```
   git clone <repository_url>
   ```

3. Navigate to the project directory:

   ```
   cd helloworld_project
   ```

4. Run the Django development server:

   ```
   python manage.py runserver
   ```

5. Visit `http://127.0.0.1:8000/` in your web browser to access the Hello World JSON response.

## Optional: Rendering Hello World HTML

If you want to render the "Hello World" message in HTML, follow these additional steps:

1. Ensure you have created an HTML template named `hello_world.html` in the `helloworld_app/templates` directory. You can use the provided template in the project.

2. Modify the `hello_world` view function in `helloworld_app/views.py` to render the HTML template:

   ```python
   from django.shortcuts import render

   def hello_world(request):
       return render(request, 'hello_world.html')
   ```

3. Restart the Django development server if it's already running, and visit `http://127.0.0.1:8000/` again to see the Hello World message rendered in HTML.

## Repository Structure

- `helloworld_project/`: Django project directory.
- `helloworld_app/`: Django app directory.
- `README.md`: This file.

## Author

Bharath Kumar Pola