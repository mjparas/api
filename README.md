# API Name

API NAME: MjParas


 


## API
Description: 
The Names API is a RESTful web service that allows users to interact with a database of names. It provides various endpoints for retrieving, adding, updating, and deleting names in the database.


 


## API
Endpoints:
/getName/{lname}/{fname}:

Function: Retrieves a greeting with a concatenated full name.
HTTP Method: GET
Required Parameters: fname and lname in the URL path.
Example Usage: GET /getName/John/Doe
/postName:

Function: Adds a new name to the database.
HTTP Method: POST
Required Parameters: JSON payload with fname and lname.
Example Usage: POST /postName
/getName:

Function: Retrieves a list of names from the database.
HTTP Method: GET
Required Parameters: None
Example Usage: GET /getName
/updateName:

Function: Updates an existing name in the database.
HTTP Method: POST
Required Parameters: JSON payload with id, fname, and lname.
Example Usage: POST /updateName
/deleteName:

Function: Deletes a name from the database.
HTTP Method: POST
Required Parameters: JSON payload with id.
Example Usage: POST /deleteName



 


## Request
Payload


Explain the
structure of the request payload, including any required or optional fields.
You can use JSON examples to illustrate.


 


## Response


Describe the
structure of the API response, including possible status codes and JSON
examples.


 


## Usage


Provide code
examples or instructions on how to use your API.


 


## License


Mention the
license under which your API is distributed.


 


## Contributors


List
contributors or give credit to any external libraries or resources used.


 


## Contact
Information
