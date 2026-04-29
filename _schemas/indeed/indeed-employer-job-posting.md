---
description: A job posting on Indeed with all associated metadata including title, description, location, salary, benefits, qualifications, and application configuration.
layout: schema
name: JobPosting
properties_list:
- description: A unique identifier for the job posting within the source system. Used in combination with sourceName for upsert operations.
  name: jobPostingId
  type: string
- description: The title of the job posting. Maximum length of 75 characters.
  name: title
  type: string
- description: The full description of the job posting including responsibilities, requirements, and other details. Must be between 30 and 20,000 characters.
  name: description
  type: string
- description: Benefits offered with the position.
  name: benefits
  type: array
- description: Required or preferred qualifications for the position.
  name: qualifications
  type: array
- description: The type of employment.
  name: employmentType
  type: string
- description: The remote work policy for the position.
  name: remoteWorkPolicy
  type: string
- description: Reference to the employer posting this job.
  name: employer
  type: object
- description: The current status of the job posting on Indeed.
  name: status
  type: string
- description: The URL where candidates can apply for the position.
  name: applicationUrl
  type: string
- description: The timestamp when the job posting was created.
  name: createdAt
  type: string
- description: The timestamp when the job posting was last updated.
  name: updatedAt
  type: string
- description: The timestamp when the job posting expires.
  name: expiresAt
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-job-posting-schema.json
slug: indeed-employer-job-posting
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobPosting\",\n  \"type\": \"object\",\n  \"description\": \"A job posting on Indeed with all associated metadata including title, description, location, salary, benefits, qualifications, and application configuration.\",\n  \"properties\": {\n    \"jobPostingId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the job posting within the source system. Used in combination with sourceName for upsert operations.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the job posting. Maximum length of 75 characters.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The full description of the job posting including responsibilities, requirements, and other details. Must be between 30 and 20,000 characters.\"\n    },\n    \"benefits\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Benefits offered with the position.\"\n    },\n    \"qualifications\": {\n      \"type\": \"array\",\n      \"description\": \"Required or preferred qualifications for the position.\"\n    },\n    \"employmentType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of employment.\"\n    },\n    \"remoteWorkPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"The remote work policy for the position.\"\n    },\n    \"employer\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the employer posting this job.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the job posting on Indeed.\"\n    },\n    \"applicationUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL where candidates can apply for the position.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp when the job posting was created.\"\n    },\n    \"updatedAt\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The timestamp when the job posting was last updated.\"\n    },\n    \"expiresAt\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp when the job posting expires.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-job-posting-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: JobPosting
---
