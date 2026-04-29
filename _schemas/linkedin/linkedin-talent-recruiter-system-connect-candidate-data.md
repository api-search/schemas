---
description: CandidateData from LinkedIn API
layout: schema
name: CandidateData
properties_list:
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: middleInitial
  type: string
- description: ''
  name: prefix
  type: string
- description: ''
  name: suffix
  type: string
- description: ''
  name: emailAddresses
  type: array
- description: ''
  name: phoneNumbers
  type: array
- description: ''
  name: addresses
  type: array
- description: ''
  name: currentCompanyName
  type: string
- description: ''
  name: currentJobTitle
  type: string
- description: ''
  name: externalProfileUrl
  type: string
- description: ''
  name: atsCreatedAt
  type: integer
- description: ''
  name: atsLastModifiedAt
  type: integer
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-recruiter-system-connect-candidate-data-schema.json
slug: linkedin-talent-recruiter-system-connect-candidate-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-candidate-data-schema.json\",\n  \"title\": \"CandidateData\",\n  \"description\": \"CandidateData from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"type\": \"string\",\n      \"example\": \"John\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"example\": \"Doe\"\n    },\n    \"middleInitial\": {\n      \"type\": \"string\",\n      \"example\": \"M\"\n    },\n    \"prefix\": {\n      \"type\": \"string\",\n      \"example\": \"Mr\"\n    },\n    \"suffix\": {\n      \"type\": \"string\",\n      \"example\": \"Jr\"\n    },\n    \"emailAddresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"email\"\n      },\n      \"example\": [\n        \"john.doe@example.com\"\
  \n      ]\n    },\n    \"phoneNumbers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PhoneNumber\"\n      }\n    },\n    \"addresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Address\"\n      }\n    },\n    \"currentCompanyName\": {\n      \"type\": \"string\",\n      \"example\": \"Tech Corp\"\n    },\n    \"currentJobTitle\": {\n      \"type\": \"string\",\n      \"example\": \"Senior Software Engineer\"\n    },\n    \"externalProfileUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://example.com/profile/johndoe\"\n    },\n    \"atsCreatedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1702693664000\n    },\n    \"atsLastModifiedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1702693664000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-candidate-data-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: CandidateData
---
