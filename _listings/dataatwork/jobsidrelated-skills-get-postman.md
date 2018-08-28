{
  "info": {
    "name": "Open Skills API Skills Associated with a Job",
    "_postman_id": "5ca020a0-9648-4e9d-ae46-c63206f9aab4",
    "description": "Retrieves a collection of skills associated with a specified job.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "skills",
      "item": [
        {
          "id": "c416c623-2772-407b-aebd-d6a2f09bc10c",
          "name": "retrieves-a-collection-of-skills-associated-with-a-specified-job",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "jobs/:id/related_skills"
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
            "description": "Retrieves a collection of skills associated with a specified job"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "983f0230-a7ad-41ec-a09d-2d52ef95173e"
            }
          ]
        }
      ]
    }
  ]
}