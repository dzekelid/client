{
  "info": {
    "name": "AWS Cognito API Describe User Pool Client",
    "_postman_id": "ededb189-77fd-42b4-bcf8-25aa18d9bdda",
    "description": "Client method for returning the configuration information and metadata of the\n            specified user pool client.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "729d9283-0f21-4846-84b2-67bdee1989b3",
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
              "id": "63ec4bb5-dbab-4acf-a0bf-b3ef47686539"
            }
          ]
        },
        {
          "id": "470ad639-f120-4f54-8812-35c36f3ebd94",
          "name": "describeUserPoolClient",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUserPoolClient?ClientId=ClientId&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Client method for returning the configuration information and metadata of the\n            specified user pool client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "430838e8-d823-4904-959e-e4361e18280e"
            }
          ]
        }
      ]
    }
  ]
}