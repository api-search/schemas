---
description: CalculatedMetricList schema
layout: schema
name: CalculatedMetricList
properties_list:
- description: ''
  name: content
  type: array
- description: ''
  name: totalElements
  type: integer
- description: ''
  name: totalPages
  type: integer
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/analytics-api-calculated-metric-list-schema.json
slug: analytics-api-calculated-metric-list
source_filename: analytics-api-calculated-metric-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/analytics-api-calculated-metric-list-schema.json\",\n  \"title\": \"CalculatedMetricList\",\n  \"description\": \"CalculatedMetricList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"rsid\": {\n            \"type\": \"string\"\n          },\n          \"owner\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"integer\"\n              },\n              \"name\": {\n\
  \                \"type\": \"string\"\n              }\n            }\n          },\n          \"polarity\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"positive\",\n              \"negative\"\n            ]\n          },\n          \"definition\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    },\n    \"totalElements\": {\n      \"type\": \"integer\"\n    },\n    \"totalPages\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/analytics-api-calculated-metric-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: CalculatedMetricList
---
