{
  "info": {
    "name": "Open Skills API Skill Name Autocomplete",
    "_postman_id": "4bebccec-16a9-454a-ac29-568df28e0c1c",
    "description": "Retrieves the names, descriptions, and UUIDs of all skills matching a given search criteria.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "skill",
      "item": [
        {
          "id": "d2f30ece-5117-4b24-841d-35c1dbdbd548",
          "name": "retrieves-the-names-descriptions-and-uuids-of-all-skills-matching-a-given-search-criteria",
          "request": {
            "url": "http://api.dataatwork.org/v1/skills/autocomplete?begins_with=%7B%7D&contains=%7B%7D&ends_with=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the names, descriptions, and UUIDs of all skills matching a given search criteria"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abfd2827-7ae7-43ff-9e42-42f41525eb12"
            }
          ]
        }
      ]
    }
  ]
}