Book Management API

This is a RESTful API for managing books. It allows users to perform CRUD (Create, Read, Update, Delete) operations on books, storing the data in a MongoDB database.

API Endpoints

-------------------------------------------------------------------------------------------------------------------------
1. Add a New Book
URL: /createNewBook
Method: POST

Request Body : 
{
  "title": "The Book Title",
  "author": "Author Name",
  "summary": "Book summary or description"
}

Response: The created book object.

-------------------------------------------------------------------------------------------------------------------------

2. View a List of All Books
URL: /books
Method: GET
Response: An array of book objects.

-------------------------------------------------------------------------------------------------------------------------

3. View Details of a Specific Book by ID
URL: /books/:id
Method: GET
Response: The book object with the specified ID.

-------------------------------------------------------------------------------------------------------------------------

4. Update a Book's Details
   
URL: /books/:id
Method: PUT

Request Body:
{
  "title": "Updated Book Title",
  "author": "Updated Author Name",
  "summary": "Updated book summary or description"
}
Response: The updated book object.

-------------------------------------------------------------------------------------------------------------------------
5. Delete a Book
URL: /books/:id
Method: DELETE
Response: The deleted book object.

-------------------------------------------------------------------------------------------------------------------------

Setting Up and Running the Application Locally
Follow these steps to set up and run the application locally:

1  Clone the repository:
git clone https://github.com/Anmolkadam369/companyProject.git
cd companyProject

2 install dependencies 
npm install

3 run the code
npx nodemon 

