---
description: Registration of an employer for Candidate Sync integration, enabling candidate data synchronization between the ATS and Indeed.
layout: schema
name: EmployerRegistration
properties_list:
- description: The employer's unique identifier.
  name: employerId
  type: string
- description: The current registration status.
  name: registrationStatus
  type: string
- description: Enabled Candidate Sync features for this employer.
  name: features
  type: array
- description: When the employer was registered for Candidate Sync.
  name: registeredAt
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-employer-registration-schema.json
slug: indeed-employer-employer-registration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmployerRegistration\",\n  \"type\": \"object\",\n  \"description\": \"Registration of an employer for Candidate Sync integration, enabling candidate data synchronization between the ATS and Indeed.\",\n  \"properties\": {\n    \"employerId\": {\n      \"type\": \"string\",\n      \"description\": \"The employer's unique identifier.\"\n    },\n    \"registrationStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current registration status.\"\n    },\n    \"features\": {\n      \"type\": \"array\",\n      \"description\": \"Enabled Candidate Sync features for this employer.\"\n    },\n    \"registeredAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the employer was registered for Candidate Sync.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-employer-registration-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: EmployerRegistration
---
