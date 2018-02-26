---
swagger: "2.0"
info:
  title: Open Skills API
  description: A complete and standard data store for canonical and emerging skills,
    knowledge, abilities, tools, technolgies, and how they relate to jobs.
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
  /skills:
    get:
      summary: Skill Names and Descriptions
      description: Retrieve the names, descriptions, and UUIDs of all skills
      operationId: retrieve-the-names-descriptions-and-uuids-of-all-skills
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
      - skills
definitions:
  Jobs:
    properties:
      links:
        description: This is a default description.
        type: string
  Job:
    properties:
      uuid:
        description: This is a default description.
        type: string
      title:
        description: This is a default description.
        type: string
      normalized_job_title:
        description: This is a default description.
        type: string
      parent_uuid:
        description: This is a default description.
        type: string
  JobSkills:
    properties:
      job_uuid:
        description: This is a default description.
        type: string
      job_title:
        description: This is a default description.
        type: string
      normalized_job_title:
        description: This is a default description.
        type: string
      skills:
        description: This is a default description.
        type: string
  NormalizedJob:
    properties:
      uuid:
        description: This is a default description.
        type: string
      title:
        description: This is a default description.
        type: string
      relevance_score:
        description: This is a default description.
        type: string
      parent_uuid:
        description: This is a default description.
        type: string
  JobSkill:
    properties:
      job_uuid:
        description: This is a default description.
        type: string
      job_title:
        description: This is a default description.
        type: string
      normalized_job_title:
        description: This is a default description.
        type: string
      importance:
        description: This is a default description.
        type: string
      level:
        description: This is a default description.
        type: string
  JobRelatedJobs:
    properties:
      uuid:
        description: This is a default description.
        type: string
      related_job_titles:
        description: This is a default description.
        type: string
  JobRelatedJob:
    properties:
      uuid:
        description: This is a default description.
        type: string
      title:
        description: This is a default description.
        type: string
      parent_uuid:
        description: This is a default description.
        type: string
  Skills:
    properties:
      links:
        description: This is a default description.
        type: string
  Skill:
    properties:
      uuid:
        description: This is a default description.
        type: string
      name:
        description: This is a default description.
        type: string
      onet_element_id:
        description: This is a default description.
        type: string
      normalized_skill_name:
        description: This is a default description.
        type: string
  NormalizedSkill:
    properties:
      uuid:
        description: This is a default description.
        type: string
      skill_name:
        description: This is a default description.
        type: string
  SkillJobs:
    properties:
      skill_uuid:
        description: This is a default description.
        type: string
      skill_name:
        description: This is a default description.
        type: string
      normalized_job_title:
        description: This is a default description.
        type: string
      jobs:
        description: This is a default description.
        type: string
  SkillJob:
    properties:
      skill_uuid:
        description: This is a default description.
        type: string
      skill_name:
        description: This is a default description.
        type: string
      description:
        description: This is a default description.
        type: string
      normalized_skill_name:
        description: This is a default description.
        type: string
      importance:
        description: This is a default description.
        type: string
      level:
        description: This is a default description.
        type: string
  SkillRelatedSkills:
    properties:
      uuid:
        description: This is a default description.
        type: string
      related_skill_name:
        description: This is a default description.
        type: string
  SkillRelatedSkill:
    properties:
      uuid:
        description: This is a default description.
        type: string
      skill_name:
        description: This is a default description.
        type: string
  PageLink:
    properties:
      rel:
        description: This is a default description.
        type: string
      href:
        description: This is a default description.
        type: string
  Error:
    properties:
      code:
        description: This is a default description.
        type: string
      message:
        description: This is a default description.
        type: string
x-collection-name: DataAtWork
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