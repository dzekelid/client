{
  "info": {
    "name": "AWS Cognito API Create User Pool Client",
    "_postman_id": "94927589-1556-47d0-b804-8067391877a9",
    "description": "Creates the user pool client.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "adddcccc-139f-4c92-ae3b-030a8bc0e859",
          "name": "createUserPoolClient",
          "request": {
            "url": "http://example.com/api/?Action=CreateUserPoolClient?ClientName=ClientName&ExplicitAuthFlows=ExplicitAuthFlows&GenerateSecret=GenerateSecret&ReadAttributes=ReadAttributes&RefreshTokenValidity=RefreshTokenValidity&UserPoolId=UserPoolId&WriteAttributes=WriteAttributes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates the user pool client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68992a04-f60d-4e28-a4c2-304942334fae"
            }
          ]
        }
      ]
    }
  ]
}