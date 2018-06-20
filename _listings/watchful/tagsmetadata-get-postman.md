{
  "info": {
    "name": "Watchful Get The List Of Fields",
    "_postman_id": "78f58792-e978-464a-a668-7b14c97dccfa",
    "description": "Returns a list of fields",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Audits",
      "item": [
        {
          "id": "5cd16f4a-c477-4e37-8d25-57b673ef0efe",
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
              "id": "55cf5a2f-d8d2-4cfd-a1f1-f5220b2d83a1"
            }
          ]
        }
      ]
    },
    {
      "name": "Extensions",
      "item": [
        {
          "id": "852d0a64-580f-4ab3-a118-cf36028a7c5d",
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
              "id": "faf5873c-e0a4-40d0-b343-a38b5f446160"
            }
          ]
        }
      ]
    },
    {
      "name": "Feedbacks",
      "item": [
        {
          "id": "014aef31-e85d-4273-9b68-691dad7ed0fc",
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
              "id": "e421353b-7107-4d58-9822-45cdead01805"
            }
          ]
        }
      ]
    },
    {
      "name": "Logs",
      "item": [
        {
          "id": "5ba35706-0045-4ceb-bada-39851e5d93b3",
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
              "id": "8feb2643-7a93-4bc6-b38e-0598202a4ec7"
            }
          ]
        }
      ]
    },
    {
      "name": "Sites",
      "item": [
        {
          "id": "e5707732-a6a2-4d79-9863-c85874a9eadb",
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
              "id": "c26825d6-9015-49dc-b53a-cd24932bcac5"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "e2260c3b-f3d4-463b-9d0d-6a04fd508b30",
          "name": "tags.metadata.get",
          "request": {
            "url": "http://watchful.li/api/v1/tags/metadata",
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
              "id": "d46b3d3c-f15e-4ec1-8127-3789182f6494"
            }
          ]
        }
      ]
    }
  ]
}