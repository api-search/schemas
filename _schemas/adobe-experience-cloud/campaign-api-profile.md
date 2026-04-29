---
description: Profile schema
layout: schema
name: Profile
properties_list:
- description: ''
  name: PKey
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: birthDate
  type: string
- description: ''
  name: phone
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: lastModified
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/campaign-api-profile-schema.json
slug: campaign-api-profile
source_filename: campaign-api-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-profile-schema.json\",\n  \"title\": \"Profile\",\n  \"description\": \"Profile schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PKey\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"birthDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"phone\": {\n      \"type\": \"string\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-profile-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Profile
---
