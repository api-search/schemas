---
description: PropertyList schema
layout: schema
name: PropertyList
properties_list:
- description: ''
  name: properties
  type: array
- description: ''
  name: type
  type: object
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/target-api-property-list-schema.json
slug: target-api-property-list
source_filename: target-api-property-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-property-list-schema.json\",\n  \"title\": \"PropertyList\",\n  \"description\": \"PropertyList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"token\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"type\": \"object\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-property-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: PropertyList
---
