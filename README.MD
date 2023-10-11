"# api"

# API Name

JSON POST

This JSON POST API endpoint lets clients transmit structured data to a server to create or update records. The request body transmits JSON data, making it adaptable and easy to work with. The server returns an HTTP status code and necessary JSON after processing. It can be used for user registration, data updates, and bespoke workflows with secure authentication. Reference proper documentation for endpoint requirements and error-handling procedures.

## API

API streamlines operations, offering seamless data management, real-time communication, and secure integration with third-party services. With robust authentication, scalable architecture, and comprehensive documentation, it empowers developers to create versatile and efficient applications. Experience enhanced functionality and superior user engagement with API.

Purpose:
API is crafted to simplify complex processes and enhance the functionality of your applications. Whether you are developing a website, mobile app, or any other software, our API offers a robust set of tools to streamline operations, improve user experience, and boost productivity.

Key Features:

Data Management:

- Easily store, retrieve, and manage data using our API. It supports various data types and formats, ensuring compatibility with different systems.
- Secure data transmission and storage protocols to safeguard sensitive information.

Authentication and Authorization:

- Implement secure user authentication and authorization mechanisms to protect your API endpoints.
-Fine-grained access control to restrict user actions based on roles and permissions.

Real-time Communication:

- Enable real-time communication between users with features like instant messaging, notifications, and live updates.
- WebSockets and other protocols for efficient real-time data exchange.

Integration with Third-party Services:

- Seamlessly integrate with popular third-party services, allowing you to leverage external functionalities without leaving your application.
- Social media, payment gateways, mapping services, and more.

Analytics and Reporting:

- Generate detailed analytics and reports to gain valuable insights into user behavior, system performance, and other crucial metrics.
- Customizable reporting tools to visualize data according to your specific requirements.

Scalability and Reliability:

- Highly scalable architecture to accommodate growing user demands without compromising performance.
-Redundancy and failover mechanisms to ensure uninterrupted service even in case of server failures.

Documentation and Support:

- Comprehensive API documentation with detailed endpoints, request methods, and response formats.
-Dedicated customer support to assist you in API integration, issue resolution, and updates.

Security:

- Implement industry-standard security protocols such as HTTPS, OAuth, and API keys.
- Regular security audits and updates to protect against emerging threats.

Customization:

- Customize API endpoints and functionalities according to your specific use case and business requirements.
- Flexible configuration options to adapt the API to your application's unique needs.

Error Handling:

- Clear and concise error messages to facilitate easy debugging and troubleshooting.
- Predictive error handling to preemptively address potential issues.

API is designed to empower developers, businesses, and entrepreneurs by providing a robust foundation for their applications. Whether you are building a social networking platform, e-commerce website, or productivity app, our API is the key to unlocking limitless possibilities. Experience enhanced functionality, improved user engagement, and unparalleled efficiency with our API today.

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

3. Send a POST Request to Update Data:
To update existing database entries using the /api/public/postUpdate endpoint:

Select the HTTP method as POST.
Enter the URL: http://127.0.0.1/api/public/postUpdate.
In the request body, include the parameters id, fname, and lname, along with the updated values.
Click "Send" to submit the request.

4. Send a POST Request to Print Data:
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
- agtarap.ivan03@gmail.com
- dustinivan.agtarap@student.dmmmsu.edu.ph
- 09480777611

