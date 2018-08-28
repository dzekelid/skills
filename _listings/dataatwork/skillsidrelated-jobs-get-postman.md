{
  "info": {
    "name": "Open Skills API Jobs Associated with a Skill",
    "_postman_id": "dca36f6c-132d-4e28-b182-d9ba8e3c8d2f",
    "description": "Retrieves a collection of jobs associated with a specified skill.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "jobs",
      "item": [
        {
          "id": "244d5af2-70a0-4f4a-a288-da05d97fe6bc",
          "name": "retrieves-a-collection-of-jobs-associated-with-a-specified-skill",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "skills/:id/related_jobs"
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
            "description": "Retrieves a collection of jobs associated with a specified skill"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2b6f080-73f3-4297-9e30-7ca88e1fd93b"
            }
          ]
        }
      ]
    }
  ]
}