"# api"

# API Name

JSON POST


 

## API
Description

This JSON POST API endpoint lets clients transmit structured data to a server to create or update records. The request body transmits JSON data, making it adaptable and easy to work with. The server returns an HTTP status code and necessary JSON after processing. It can be used for user registration, data updates, and bespoke workflows with secure authentication. Reference proper documentation for endpoint requirements and error-handling procedures.



## API
Endpoints

Explain the accessible endpoints, their roles, and the necessary inputs.

http://127.0.0.1/api/public/postName

Purpose: This endpoint is designed to add new information to the database.
Required Parameters: First name (fname), Last name (lname).

http://127.0.0.1/api/public/postUpdate

Purpose: This endpoint is utilized for modifying existing data in the database.
Required Parameters: ID, First name (fname), Last name (lname).

http://127.0.0.1/api/public/postPrint

Purpose: This endpoint serves the function of displaying the data stored in the database.
Required Parameters: None.

http://127.0.0.1/api/public/postDelete

Purpose: This endpoint is responsible for removing specific data from the database.
Required Parameters: ID.



## Request
Payload

JSON Payload postName:

Request payload:
- {
  "lname":"hortizuela",
   "fname":"manny"
}

 JSON Payload printName:
 
Request payload:

JSON Payload updateName:

Request payload:
- {
  "id":1,
  "lname":"wick",
   "fname":"john"
}

JSON Payload deleteName:

Request payload:
- {
  "id":1
}

## Response
JSON Payload postName:

- Response payload:
- {
         "status":"success","data":null
}

JSON Payload printName:

- Response payload:
- {
         "status":"success","data":["lname":"hortizuela","fname":"manny","lname":"licayan","fname":"arnold"]
}


JSON Payload updateName:

- Response payload:
- {
         "status":"success","data":null
}


JSON Payload deleteName:

- Response payload:
- {
         "status":"success","data":null
}




## Usage

Follow these steps to manipulate database information using Postman and the API endpoints:

1. Launch Postman:
Ensure that Postman is installed and operational on your system.

2. Send a POST Request to Insert Data:
To insert data into the database via the /api/public/postName endpoint:

Choose the HTTP method as POST.
Input the URL: http://127.0.0.1/api/public/postName.
Within the request body, specify the parameters fname and lname along with the desired values for insertion.
Click "Send" to dispatch the request.

3.Send a POST Request to Update Data:
To update existing database entries using the /api/public/postUpdate endpoint:

Select the HTTP method as POST.
Enter the URL: http://127.0.0.1/api/public/postUpdate.
In the request body, include the parameters id, fname, and lname, along with the updated values.
Click "Send" to submit the request.

4.Send a POST Request to Print Data:
To showcase database data using the /api/public/postPrint endpoint:

Opt for the HTTP method as POST.
Specify the URL: http://127.0.0.1/api/public/postPrint.
Keep the request body empty as no additional parameters are required.
Click "Send" to transmit the request.

5. Send a POST Request to Delete Data:
To remove data from the database through the /api/public/postDelete endpoint:

Set the HTTP method to POST.
Enter the URL: http://127.0.0.1/api/public/postDelete.
In the request body, include the parameter id with the ID of the data you intend to delete.

Click "Send" to initiate the request.
 

## License

No License 


## Contributors

Sir Manny Hortizuela
provided:

- some codes
- database structure
- payloads
- etc.


## Contact
Include contact
information for inquiries or support.

Dustin Ivan Z. Agtarap 
- dustinivan.agtarap@student.dmmmsu.edu.ph
- 09480777611

