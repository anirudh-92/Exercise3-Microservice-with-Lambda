# Exercise3-Microservice-with-Lambda

Created a simple backend (read/write to DynamoDB) with a RESTful API endpoint using Amazon API Gateway.

To create API and Lambda function: 

  - Choose Use a blueprint.
  - Choose the microservice-http-endpoint blueprint.
  - Name – lambda-microservice.
  - Role – Create a new role from AWS policy templates.
  - Role name – lambda-apigateway-role.
  - Policy templates – Simple microservice permissions.
  - API – Create an API.
  - API Type – HTTP API.
  - Security – Open.
  - Created the function: lambda-microservice.

To create a DynamoDB table
- Create a table with the following settings.
- Table name – mytable-stream
- Primary key – id (string)

To enable streams
- Choose Tables.
- Choose the lambda-dynamodb-stream table.
- Under Exports and streams, choose DynamoDB stream details.
- Choose Enable stream.

Test:


<img width="1027" alt="Screenshot 2022-08-15 at 10 41 05" src="https://user-images.githubusercontent.com/100350582/184613330-158cafcc-0b69-489c-99d5-4a2832d2293a.png">
<img width="1050" alt="Screenshot 2022-08-15 at 10 41 20" src="https://user-images.githubusercontent.com/100350582/184613336-c8f5bfe0-1aef-47e2-b2c1-359c9dcb1825.png">
