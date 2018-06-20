{
  "info": {
    "name": "HHS Media Services Get Youtube metadata for MediaItem",
    "_postman_id": "c12ca736-80c8-47fa-8a11-df9af1809705",
    "description": "Returns the Youtube metadata, where applicable, for the MediaItem identified by the 'id'.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "f7c1d15c-bc54-4750-abff-cd7d065cfaa3",
          "name": "getMediaYoutubeMetaDataById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/media/:id/youtubeMetaData.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the Youtube metadata, where applicable, for the MediaItem identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e53ee49a-5ad8-424c-ada5-b2cd2f7f92bc"
            }
          ]
        }
      ]
    }
  ]
}