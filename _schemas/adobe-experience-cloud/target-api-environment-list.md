---
description: EnvironmentList schema
layout: schema
name: EnvironmentList
properties_list:
- description: ''
  name: environments
  type: array
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/target-api-environment-list-schema.json
slug: target-api-environment-list
source_filename: target-api-environment-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-environment-list-schema.json\",\n  \"title\": \"EnvironmentList\",\n  \"description\": \"EnvironmentList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-environment-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: EnvironmentList
---
