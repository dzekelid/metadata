{
  "info": {
    "name": "Watchful Get The List Of Fields",
    "_postman_id": "cca41a08-375f-491f-abb9-392b9afc5751",
    "description": "Returns a list of fields",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Audits",
      "item": [
        {
          "id": "f393109b-2fc7-4c44-ad16-ee60b3030c42",
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
              "id": "d78c306b-eea4-4ece-bc9e-779e7e8c6e03"
            }
          ]
        }
      ]
    },
    {
      "name": "Extensions",
      "item": [
        {
          "id": "673278d4-8715-41a3-9e08-a419ab8bbbef",
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
              "id": "57ca7d83-6e53-4268-8e2d-6e18c76b047e"
            }
          ]
        }
      ]
    },
    {
      "name": "Feedbacks",
      "item": [
        {
          "id": "fe69f497-c83f-4b4c-b18b-68aa4617e70c",
          "name": "getFieldsFeedbacks",
          "request": {
            "url": "http://watchful.li/api/v1/feedbacks/metadata",
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
              "id": "2927db56-b9bf-4c16-b078-6fe7d2dcd12f"
            }
          ]
        }
      ]
    },
    {
      "name": "Logs",
      "item": [
        {
          "id": "bcfaaad2-6ba9-47a6-8846-bcfc0cf99ee6",
          "name": "getFieldsLogs",
          "request": {
            "url": "http://watchful.li/api/v1/logs/metadata",
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
              "id": "b9272b93-da8e-472d-80b4-83612bc8cf7b"
            }
          ]
        }
      ]
    }
  ]
}