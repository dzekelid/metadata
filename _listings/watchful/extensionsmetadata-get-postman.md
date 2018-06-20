{
  "info": {
    "name": "Watchful Get The List Of Fields",
    "_postman_id": "7aacbd68-ae31-4128-888a-b8db12f7393b",
    "description": "Returns a list of fields",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Audits",
      "item": [
        {
          "id": "311a15b1-fdb3-4996-8a0d-485ec9cbbfb0",
          "name": "getFieldsAudits",
          "request": {
            "url": "http://watchful.li/api/v1/audits/metadata",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of fields"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74da9eeb-40a0-4446-80c8-5f7beedc52eb"
            }
          ]
        }
      ]
    },
    {
      "name": "Extensions",
      "item": [
        {
          "id": "0af333b4-2ae0-4653-b274-07f1bbebb978",
          "name": "getFieldsExtensions",
          "request": {
            "url": "http://watchful.li/api/v1/extensions/metadata",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of fields"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aad9640e-95d5-4537-ae48-8ac12a2dad4c"
            }
          ]
        }
      ]
    }
  ]
}