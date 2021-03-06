# LibraryServer

## Product Description
This is the front and back end code for Gray's original back end LibraryServer project that can be found here:
https://github.com/gdodgen/LibraryServer
Minor changes have been made on the backend.
This code is packaged onto Tomcat being run on an Amazon Linux EC2 Server.
The data is connected to an Amazon RDS.  
The purpose of the front end is to allow users to see a list of books which the user can add/edit/delete. 

## Technologies Used
* HTML
* CSS
* JavaScript
* Java Servlets
* Tomcat
* Jenkins
* AWS EC2
* AWS RDS
* PostgreSQL

## Features
### Ready Features
1. See a list of books.
2. Add a book by clicking on the "Add Book" link in the navbar. 
3. Edit a book by clicking the "Edit" button on the table with the corresponding row.
4. Delete a book by clicking the "X" button on the table with the corresponding row. 

### Planned Improvements
1. Filter book results by author/genre/title.
2. Make the site more asthetically pleasing. 
3. Allow for checking in/out books by users.
4. Allow users to see which books they have checked out. 
5. Add due dates to books based on when the books are checked out.
6. Allow new users to create an account.  

## Jenkins
The project has one Jenkins pipeline called "Git Pull Pipeline"
When the pipeline is ran, Jenkins will do a pull request from the Library Server GitHub repo at:
https://github.com/yasmine-sorhovigarat/LibraryServer
It will then package the new code and deploy it on the Tomcat server.

## Getting Started
Clone the code onto your machine.
Requirements: Java 8 SDK, Maven 3.5.2, and Tomcat 9
Import the project as an existing maven project. 
Update depenedencies and run mvn clean package.
Deploy the war file in the target folder on Tomcat's webapp folder.
Start the Tomcat server.

## Usage Home Page  
http://localhost:8080/LibraryServer/static/index.html
or
{ip-address}:{port}/LibraryServer/static/index.html
For example: http://3.129.148.58:8080/LibraryServer/static/index.html

## Contributors
* Yasmine Sorhovigarat
* Gray Dodgen

## Lincense
None
