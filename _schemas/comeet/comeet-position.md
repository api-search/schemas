---
description: Schema for a single published job position retrieved from the Comeet Careers API.
layout: schema
name: Comeet Position
properties_list:
- description: Unique identifier for the position.
  name: uid
  type: string
- description: Job title.
  name: name
  type: string
- description: ''
  name: department
  type: string
- description: ''
  name: company_department
  type: string
- description: ''
  name: location
  type: object
- description: ''
  name: url_active_after
  type: string
- description: ''
  name: url_comeet_hosted_page
  type: string
- description: ''
  name: details
  type: object
- description: ''
  name: status
  type: string
provider_name: Comeet
provider_slug: comeet
schema_file: json-schema/comeet-position-schema.json
slug: comeet-position
source_filename: comeet-position-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/comeet/refs/heads/main/json-schema/comeet-position-schema.json\",\n  \"title\": \"Comeet Position\",\n  \"description\": \"Schema for a single published job position retrieved from the Comeet Careers API.\",\n  \"type\": \"object\",\n  \"required\": [\"uid\", \"name\"],\n  \"properties\": {\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the position.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Job title.\"\n    },\n    \"department\": {\n      \"type\": \"string\"\n    },\n    \"company_department\": {\n      \"type\": \"string\"\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"country\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n\
  \    \"url_active_after\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"url_comeet_hosted_page\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"details\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"description\": { \"type\": \"string\" },\n        \"requirements\": { \"type\": \"string\" }\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"published\", \"draft\", \"archived\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/comeet/refs/heads/main/json-schema/comeet-position-schema.json
tags:
- ATS
- Candidates
- Careers
- Interviews
- Jobs
- Recruiting
- Talent Acquisition
title: Comeet Position
---
