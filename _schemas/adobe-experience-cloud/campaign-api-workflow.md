---
description: Workflow schema
layout: schema
name: Workflow
properties_list:
- description: ''
  name: PKey
  type: string
- description: ''
  name: label
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: startDate
  type: string
- description: ''
  name: created
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/campaign-api-workflow-schema.json
slug: campaign-api-workflow
source_filename: campaign-api-workflow-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-workflow-schema.json\",\n  \"title\": \"Workflow\",\n  \"description\": \"Workflow schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PKey\": {\n      \"type\": \"string\"\n    },\n    \"label\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"started\",\n        \"paused\",\n        \"stopped\",\n        \"finished\",\n        \"error\"\n      ]\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-workflow-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Workflow
---
