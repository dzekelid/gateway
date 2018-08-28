{
  "info": {
    "name": "AWS Storage Gateway Service API Activate Gateway",
    "_postman_id": "af9474aa-277d-400e-ad7f-fc6616d4b055",
    "description": "Activates the gateway you previously deployed on your host.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Gateway",
      "item": [
        {
          "id": "5c27efc3-a25f-4a76-a893-32eaf8c34e14",
          "name": "activateGateway",
          "request": {
            "url": "http://example.com/api/?Action=ActivateGateway?ActivationKey=ActivationKey&GatewayName=GatewayName&GatewayRegion=GatewayRegion&GatewayTimezone=GatewayTimezone&GatewayType=GatewayType&MediumChangerType=MediumChangerType&TapeDriveType=TapeDriveType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Activates the gateway you previously deployed on your host."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca95fa4a-71ec-4c77-bfc4-0b4ba0d98ae1"
            }
          ]
        }
      ]
    }
  ]
}