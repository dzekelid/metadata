{
  "info": {
    "name": "Watchful Get The List Of Fields",
    "_postman_id": "08ae3914-a147-4219-91f9-e4e98d4db06c",
    "description": "Returns a list of fields",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Audits",
      "item": [
        {
          "id": "4592c36a-ecea-4b65-9d46-51bde37d5bfa",
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
              "id": "b83a0d85-a429-4b86-a18b-00e8163610b7"
            }
          ]
        }
      ]
    },
    {
      "name": "Extensions",
      "item": [
        {
          "id": "b4316e5c-12c5-449a-a61a-9ee70368a4e2",
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
              "id": "4ad21313-6165-4dad-9302-441715158d83"
            }
          ]
        }
      ]
    },
    {
      "name": "Feedbacks",
      "item": [
        {
          "id": "1626249a-c9cd-4b80-94b2-7840c860ca51",
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
              "id": "db3cdef1-7769-4fd3-af98-b4ad3a6db53f"
            }
          ]
        }
      ]
    },
    {
      "name": "Logs",
      "item": [
        {
          "id": "370b907e-e87f-4faa-90c1-5c0d54be014c",
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
              "id": "bc24c05d-ca7a-420a-9794-309400ac61b5"
            }
          ]
        }
      ]
    },
    {
      "name": "Sites",
      "item": [
        {
          "id": "8b7ab56a-faaa-4e8a-98ec-d0d2b5915989",
          "name": "sites.metadata.get",
          "request": {
            "url": "http://watchful.li/api/v1/sites/metadata",
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
              "id": "88ccc6d1-422d-457b-a73f-d345caae20ef"
            }
          ]
        }
      ]
    }
  ]
}