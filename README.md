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
API Payload:

Request Payload Structure:

For the /postName endpoint, the request payload should be a JSON object containing fname and lname. 
For example:
{
    "lname": "Hortizuela",
    "fname": "Manny"
}

For the /updateName endpoint, the request payload should include the id of the name to be updated along with the new fname and lname.
For example:
{
  "id":1,
  "lname":"wick",
   "fname":"john"
}

For the /deleteName endpoint, the request payload should include the id of the name to be deleted.
For example:
{
  "id":1
}


 


## Response
API Response:

The response for most endpoints contains a JSON object with a status field (either "success" or "error") and a data field. The structure of the data field varies based on the specific endpoint.

For /postName: { "status": "success", "data": null }

For /getName: { "status": "success", "data": [ {"lname": "Hortizuela", "fname": "Manny"}, {"lname": "Licayan", "fname": "Arnold"} ] }

For /updateName: { "status":"success","data":null }

For /deleteName: { "status":"success","data":null }.

 


## Usage





 


## License


Mention the
license under which your API is distributed.


 


## Contributors


List
contributors or give credit to any external libraries or resources used.


 


## Contact
Information
