---
swagger: "2.0"
x-collection-name: DataAtWork
x-complete: 0
info:
  title: Open Skills API Jobs Associated with a Skill
  description: Retrieves a collection of jobs associated with a specified skill.
  contact:
    name: Work Data Initiative
    url: http://www.dataatwork.org
  version: "1.0"
host: api.dataatwork.org
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /jobs/{id}/related_skills:
    get:
      summary: Skills Associated with a Job
      description: Retrieves a collection of skills associated with a specified job.
      operationId: retrieves-a-collection-of-skills-associated-with-a-specified-job
      x-api-path-slug: jobsidrelated-skills-get
      parameters:
      - in: path
        name: id
        description: The UUID of the job to retrieve skills for
      responses:
        200:
          description: OK
      tags:
      - Skills
      - Associated
      - Job
  /skills/{id}/related_skills:
    get:
      summary: Skills Associated with a Skill
      description: Retrieves a collection of skills associated with a specified skill.
      operationId: retrieves-a-collection-of-skills-associated-with-a-specified-skill
      x-api-path-slug: skillsidrelated-skills-get
      parameters:
      - in: path
        name: id
        description: The UUID of the skill to retrieve related skills for
      responses:
        200:
          description: OK
      tags:
      - Skills
      - Associated
      - Skill
  /skills:
    get:
      summary: Skill Names and Descriptions
      description: Retrieve the names, descriptions, and UUIDs of all skills.
      operationId: retrieve-the-names-descriptions-and-uuids-of-all-skills
      x-api-path-slug: skills-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items per page
      - in: query
        name: offset
        description: Pagination offset
      responses:
        200:
          description: OK
      tags:
      - Skill
      - Names
      - Descriptions
  /skills/{id}:
    get:
      summary: Skill Name and Description
      description: Retrieves the name, description, and UUID of a job by specifying
        its UUID.
      operationId: retrieves-the-name-description-and-uuid-of-a-job-by-specifying-its-uuid
      x-api-path-slug: skillsid-get
      parameters:
      - in: path
        name: id
        description: The UUID of the skill name to retrieve
      responses:
        200:
          description: OK
      tags:
      - Skill
      - Name
      - Description
  /skills/{id}/related_jobs:
    get:
      summary: Jobs Associated with a Skill
      description: Retrieves a collection of jobs associated with a specified skill.
      operationId: retrieves-a-collection-of-jobs-associated-with-a-specified-skill
      x-api-path-slug: skillsidrelated-jobs-get
      parameters:
      - in: path
        name: id
        description: The UUID of the skill to retrieve jobs for
      responses:
        200:
          description: OK
      tags:
      - Jobs
      - Associated
      - Skill
  /skills/autocomplete:
    get:
      summary: Skill Name Autocomplete
      description: Retrieves the names, descriptions, and UUIDs of all skills matching
        a given search criteria.
      operationId: retrieves-the-names-descriptions-and-uuids-of-all-skills-matching-a-given-search-criteria
      x-api-path-slug: skillsautocomplete-get
      parameters:
      - in: query
        name: begins_with
        description: Find skill names beginning with the given text fragment
      - in: query
        name: contains
        description: Find skill names containing the given text fragment
      - in: query
        name: ends_with
        description: Find skill names ending with the given text fragment
      responses:
        200:
          description: OK
      tags:
      - Skill
      - Name
      - Autocomplete
  /skills/normalize:
    get:
      summary: Skill Name Normalization
      description: Retrieves the canonical skill name for a synonymous skill name
      operationId: retrieves-the-canonical-skill-name-for-a-synonymous-skill-name
      x-api-path-slug: skillsnormalize-get
      parameters:
      - in: query
        name: skill_name
        description: Find the canonical skill name(s) for skills matching the given
          text fragment
      responses:
        200:
          description: OK
      tags:
      - Skill
      - Name
      - Normalization
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---