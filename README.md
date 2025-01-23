Objective:

Students will design and implement a REST API using the Crow framework in C++. The API will manage a library collection of books while integrating SQLite for persistent storage.

To manage a library system, the API will provide endpoints for:
1) Adding a book.
2) Retrieving all books.
3) Updating book details.
4) Deleting a book.

Data will be stored in an SQLite database; the project should follow proper coding and organizational practices. You can use the template on the Github repository for proper directory use.


CORE Endpoints:
1) POST /books:
2) GET /books:
3) PUT /books/{id}:
4) DELETE /books/{id}:

SQLITE:
library.db
single table: books
	columns:
		id (Primary Key, Auto-increment)
		title (Text, Required)
		autor (Text, Required)
		year (Int, Required)

ERROR Handling:
	Return appropriate HTTP status codes and messages for common errors

CODE Organization:
use GitHUB template provided. All directories are designed.

Moonshot goals for bonus points:
The above material must be done correctly with good practices for any bonus points to be awarded. Note that these bonus goals may be standard requirements for the next assignment. 

1. Search Endpoint
		Add a GET /books/search?author = author_name endpoint
		Return all books by a specific author
2. Pagination
		Add support for paginated responses in GET /books/
		return page=1&limit=5
3. Sorting
		Allow sorting results in GET /books by title or year using query parameters
		(/books?sort=year&order=asc)
4. Swagger/OpenAPI Integration
		add open API documentation for your API using a library like crow-openapi

5. Authentication
		Add a simple API key authentication system. Clients must include an "Authorization" header with a valid API key to access the endpoints

DELIVERABLES
1. Code submission: submit the complete project directory with the CMakeLists.txt, source, and the SQLite database.
2. Information on testing your API
		What are the API endpoints that are needed to be tested?
		What kind of data is needed by an API?
		What kind of response is given by an API?
		How much time an API should take to respond?
		What kind of response should an API give in case a request fails? 

DOCUMENTATION
1. Include in the README.md
	  Name and date
	  Project overview (above)
	  API endpoint details
	  Instructions to build and run the project
2. Information on testing your API
		What are the API endpoints that are needed to be tested?
		What kind of data is needed by an API?
		What kind of response is given by an API?
		How much time an API should take to respond?
		What kind of response should an API give in case a request fails? 


DEMO VIDEO
	Record a video of outlining the specific functions in the main, how the code works for specific tasks, how the CMakeLists.txt file works, and a demonstration of the API working.
