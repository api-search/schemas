---
description: An employer entity on Indeed representing a company or organization that posts jobs and manages candidates.
layout: schema
name: Employer
properties_list:
- description: A globally unique employer identifier. For ATS partners, this typically combines the ATS system identifier with the employer's internal ID.
  name: id
  type: string
- description: The display name of the employer as it appears on Indeed job listings and company pages.
  name: employerName
  type: string
- description: The type of employer entity.
  name: employerType
  type: string
- description: The timestamp when the employer was created on Indeed.
  name: createdAt
  type: string
- description: The timestamp when the employer was last updated.
  name: updatedAt
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-employer-schema.json
slug: indeed-employer-employer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Employer\",\n  \"type\": \"object\",\n  \"description\": \"An employer entity on Indeed representing a company or organization that posts jobs and manages candidates.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A globally unique employer identifier. For ATS partners, this typically combines the ATS system identifier with the employer's internal ID.\"\n    },\n    \"employerName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the employer as it appears on Indeed job listings and company pages.\"\n    },\n    \"employerType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of employer entity.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp when the employer was created on Indeed.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"The timestamp when the employer was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-employer-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: Employer
---
