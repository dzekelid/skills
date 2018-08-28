{
  "info": {
    "name": "Open Skills API Skill Name and Description",
    "_postman_id": "55c9d4d3-750b-4392-ad50-bd717585433b",
    "description": "Retrieves the name, description, and UUID of a job by specifying its UUID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Job",
      "item": [
        {
          "id": "6688c4e2-9760-4a6d-b800-8f533b286c19",
          "name": "retrieves-the-names-descriptions-and-uuids-of-all-job-titles",
          "request": {
            "url": "http://api.dataatwork.org/v1/jobs?limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the names, descriptions, and UUIDs of all job titles."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6120d8e-705b-415b-b100-b2670389badf"
            }
          ]
        },
        {
          "id": "7d72a0de-fc98-4968-8b04-0b1bbbe3dd16",
          "name": "retrieves-the-name-description-and-uuid-of-a-job-by-specifying-its-onet-soc-code-or-uuid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "jobs/:id"
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
            "description": "Retrieves the name, description, and UUID of a job by specifying its O*NET SOC Code or UUID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed57b8d2-8c91-46b9-b335-08052c842387"
            }
          ]
        },
        {
          "id": "1ddcb6e5-0999-48d2-9229-47139c97a396",
          "name": "retrieves-the-names-descriptions-and-uuids-of-all-job-titles-matching-a-given-search-criteria",
          "request": {
            "url": "http://api.dataatwork.org/v1/jobs/autocomplete?begins_with=%7B%7D&contains=%7B%7D&ends_with=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the names, descriptions, and UUIDs of all job titles matching a given search criteria."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f6ecb86-2ced-4f1c-a305-e665a196ec40"
            }
          ]
        },
        {
          "id": "fae5b458-b5b8-42b9-9c4c-85512384c42a",
          "name": "retrieves-the-canonical-job-title-for-a-synonymous-job-title",
          "request": {
            "url": "http://api.dataatwork.org/v1/jobs/normalize?job_title=%7B%7D&limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the canonical job title for a synonymous job title"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "427994cf-eeaa-4f23-ac70-33b2cf9d3a43"
            }
          ]
        }
      ]
    },
    {
      "name": "Skills",
      "item": [
        {
          "id": "37050c63-783a-417f-8d85-3d2f4f76a71b",
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
            "description": "Retrieves a collection of skills associated with a specified job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ceeb86dc-560f-436f-9cf0-9c1cf7241403"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "b0cd952f-e9c3-4066-8616-4e4976e68050",
          "name": "retrieves-a-collection-of-jobs-associated-with-a-specified-job",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "jobs/:id/related_jobs"
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
            "description": "Retrieves a collection of jobs associated with a specified job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf322254-05bc-4bc0-8194-f45a54f62f18"
            }
          ]
        }
      ]
    },
    {
      "name": "Unusual",
      "item": [
        {
          "id": "c8f3fb06-3972-4ea2-ab17-fc1e82b5961d",
          "name": "retrieves-a-list-of-unusual-job-titles-and-the-uuids-of-their-canonical-jobs",
          "request": {
            "url": "http://api.dataatwork.org/v1/jobs/unusual_titles",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of unusual job titles and the UUIDs of their canonical jobs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b68ee59-e8b1-4a3a-866f-ddfcd77b2551"
            }
          ]
        }
      ]
    },
    {
      "name": "Skill",
      "item": [
        {
          "id": "1306d8f8-2856-4ca9-9385-3d4dd06fcdf2",
          "name": "retrieve-the-names-descriptions-and-uuids-of-all-skills",
          "request": {
            "url": "http://api.dataatwork.org/v1/skills?limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the names, descriptions, and UUIDs of all skills."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbc57cdb-368c-44ef-aa2a-203053e8e536"
            }
          ]
        },
        {
          "id": "3eaa5f3c-5729-4194-ab36-a62554f34aee",
          "name": "retrieves-the-name-description-and-uuid-of-a-job-by-specifying-its-uuid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "skills/:id"
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
            "description": "Retrieves the name, description, and UUID of a job by specifying its UUID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0cbde7ff-7f87-4a94-8e9a-7267a2dfc7e2"
            }
          ]
        }
      ]
    }
  ]
}