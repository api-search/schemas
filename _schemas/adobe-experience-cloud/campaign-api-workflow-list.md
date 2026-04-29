---
description: WorkflowList schema
layout: schema
name: WorkflowList
properties_list:
- description: ''
  name: content
  type: array
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/campaign-api-workflow-list-schema.json
slug: campaign-api-workflow-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-workflow-list-schema.json\",\n  \"title\": \"WorkflowList\",\n  \"description\": \"WorkflowList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"PKey\": {\n            \"type\": \"string\"\n          },\n          \"label\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"started\",\n              \"paused\",\n              \"stopped\",\n              \"finished\",\n              \"error\"\n            ]\n          },\n          \"startDate\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n   \
  \       \"created\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-workflow-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: WorkflowList
---
