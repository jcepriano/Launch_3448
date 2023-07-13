# Launch Mod 3 Week 2 Assessment

## Questions (10 Points)

1. Define MVC and explain the purpose of each of the three parts of this pattern.

    MVC is the process of creating an application separated into three parts, the Model, View, and Controller. 
    The Model is the back-end logic. It contains the structure of the application. The View displays the content
    that correlates with the request. The Controller is what responds to HTTP requests and user interaction.

2. Explain the difference between the **New** route and the **Create** route.

    'New' creates a new object but keeps it local which means nothing gets saved to a database. 'Create' also
    creates a new object but one that gets saved to a database.

3. List all of the RESTful routes for the `employee` entity. Make sure to include the Route Name, Path, and HTTP Method for each of the routes. (2 points)

    Index, /employee, GET

    New, /employee/new, GET

    Create, /employee, POST

    Show, /employee/id, GET

    Edit, /employee/edit/id, PUT

    Update, /employee/edit/id, PATCH

    Destroy, /employee/id, DELETE
    
</br>
For the following three questions, explain both how to fix the error/bug and why the part of the code that was broken is important. (2 points each)

4. 
<img width="1213" alt="Screenshot 2023-06-13 102204" src="https://github.com/turingschool/launch-curriculum/assets/11747682/f37c233d-e7aa-483e-9f75-7c9b111811e5">
    To fix the error, in the Hotels Controller, the 'hotels' variable needs to be an argument in the 'View()' method. 


5.
<img width="1245" alt="Screenshot 2023-06-13 102555" src="https://github.com/turingschool/launch-curriculum/assets/11747682/87c9fbf7-de63-4580-9b36-8632df27b91b">
    The cshtml file was named incorrectly. It is named 'Indexes' plural while the method is named 'Index' singular.
    For the connection to be made, they have to share the same name.

6. 
<img width="1238" alt="Screenshot 2023-06-13 102856" src="https://github.com/turingschool/launch-curriculum/assets/11747682/a39b525d-ae05-463f-b724-be68aa70148c">
There is no '@' symbol so the program does not know that C# is being used in the html file

## Exercise (10 Points)

Make sure to first run `update-database` to populate the `Tourism` database used by this application.

This application already has the `Index` route for States.

Your task is to do the following:
1. Add the `Show` RESTful route to display the name and abbreviation for a particular state.
1. Add a test for your new `Show` route in the `StateCRUDTests.cs` file.
