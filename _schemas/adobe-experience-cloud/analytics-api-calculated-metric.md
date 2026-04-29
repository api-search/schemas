---
description: CalculatedMetric schema
layout: schema
name: CalculatedMetric
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: rsid
  type: string
- description: ''
  name: owner
  type: object
- description: ''
  name: polarity
  type: string
- description: ''
  name: definition
  type: object
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/analytics-api-calculated-metric-schema.json
slug: analytics-api-calculated-metric
source_filename: analytics-api-calculated-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/analytics-api-calculated-metric-schema.json\",\n  \"title\": \"CalculatedMetric\",\n  \"description\": \"CalculatedMetric schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"rsid\": {\n      \"type\": \"string\"\n    },\n    \"owner\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"polarity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"positive\",\n        \"negative\"\n      ]\n    },\n    \"definition\": {\n      \"type\": \"object\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/analytics-api-calculated-metric-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: CalculatedMetric
---
