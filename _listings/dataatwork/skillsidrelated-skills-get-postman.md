{
  "info": {
    "name": "Open Skills API Skills Associated with a Skill",
    "_postman_id": "e4ee4a96-e25f-4f9b-8d5d-20ec92445a4e",
    "description": "Retrieves a collection of skills associated with a specified skill.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "skills",
      "item": [
        {
          "id": "50c5eeba-40dc-4e3f-aa4c-16e897b7cf83",
          "name": "retrieves-a-collection-of-skills-associated-with-a-specified-skill",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "skills/:id/related_skills"
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
            "description": "Retrieves a collection of skills associated with a specified skill"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b17dcdc3-dc27-4d4d-b696-26488c313204"
            }
          ]
        }
      ]
    }
  ]
}