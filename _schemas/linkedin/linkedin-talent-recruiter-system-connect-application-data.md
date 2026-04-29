---
description: ApplicationData from LinkedIn API
layout: schema
name: ApplicationData
properties_list:
- description: ''
  name: atsCandidateId
  type: string
- description: ''
  name: atsJobPostingId
  type: string
- description: ''
  name: atsJobPostingName
  type: string
- description: ''
  name: candidateEmail
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: source
  type: string
- description: ''
  name: dispositionReason
  type: string
- description: ''
  name: atsCreatedAt
  type: integer
- description: ''
  name: atsLastModifiedAt
  type: integer
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-recruiter-system-connect-application-data-schema.json
slug: linkedin-talent-recruiter-system-connect-application-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-application-data-schema.json\",\n  \"title\": \"ApplicationData\",\n  \"description\": \"ApplicationData from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"atsCandidateId\": {\n      \"type\": \"string\",\n      \"example\": \"CAND-001\"\n    },\n    \"atsJobPostingId\": {\n      \"type\": \"string\",\n      \"example\": \"JOB-2024-001\"\n    },\n    \"atsJobPostingName\": {\n      \"type\": \"string\",\n      \"example\": \"Senior Software Engineer\"\n    },\n    \"candidateEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"example\": \"johndoe@example.com\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"example\": \"John\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"Doe\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"example\": \"Referral\"\n    },\n    \"dispositionReason\": {\n      \"type\": \"string\",\n      \"example\": \"\"\n    },\n    \"atsCreatedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1702693664000\n    },\n    \"atsLastModifiedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1702693664000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-application-data-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ApplicationData
---
