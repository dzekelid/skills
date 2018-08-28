{
  "info": {
    "name": "Open Skills API Skill Names and Descriptions",
    "_postman_id": "da95cc1a-4156-4a59-91d4-f813db66bb92",
    "description": "Retrieve the names, descriptions, and UUIDs of all skills.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Job",
      "item": [
        {
          "id": "ca8c3e33-ef46-4d42-acec-16060da13ed7",
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
              "id": "59e69251-7b6a-4ed9-a6c0-1b731814a7da"
            }
          ]
        },
        {
          "id": "4826816e-f56a-41a7-a4d0-fa6e6d1b404d",
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
              "id": "ea8b6479-9a18-4dbf-9f4e-5ccb0e68df19"
            }
          ]
        },
        {
          "id": "bb64e261-774c-4708-b544-119ef616cf38",
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
              "id": "22b514f6-627b-40fc-a9ec-cf2fc5bce342"
            }
          ]
        },
        {
          "id": "cae118d9-907b-4cf1-acf4-c3beee63bbfa",
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
              "id": "456114ae-2d24-444e-88cc-f2785b356834"
            }
          ]
        }
      ]
    },
    {
      "name": "Skills",
      "item": [
        {
          "id": "7d6c6153-20a6-4537-8430-4d1ca08f9ea0",
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
              "id": "0560fff4-4ad3-4143-b2e1-529fae6e23ad"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "6da46a8f-021f-4b1d-9d39-6573dea4a80c",
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
              "id": "4e982754-2508-4fac-966b-5a9330b4f23a"
            }
          ]
        }
      ]
    },
    {
      "name": "Unusual",
      "item": [
        {
          "id": "b0829ae6-2742-4734-b9ac-35747f1656db",
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
              "id": "43fbdae6-3da8-425f-b7e1-ba237f7c8722"
            }
          ]
        }
      ]
    },
    {
      "name": "Skill",
      "item": [
        {
          "id": "2927406e-7ee5-44ea-963f-d00962cfa300",
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
              "id": "0b0ca664-35bd-4eef-a0cb-f21c9a9cfbb8"
            }
          ]
        }
      ]
    }
  ]
}