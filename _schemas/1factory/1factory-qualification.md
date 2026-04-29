---
description: Qualification schema from 1Factory API
layout: schema
name: Qualification
properties_list:
- description: Date and time when the qualification was assessed or updated.
  name: date
  type: string
- description: Current qualification status of the supplier.
  name: status
  type: string
- description: Review status of the qualification assessment.
  name: review_status
  type: string
- description: Review frequency in months for re-qualification.
  name: frequency
  type: integer
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-qualification-schema.json
slug: 1factory-qualification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-qualification-schema.json\",\n  \"title\": \"Qualification\",\n  \"description\": \"Qualification schema from 1Factory API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": false,\n      \"description\": \"Date and time when the qualification was assessed or updated.\",\n      \"example\": \"2016-11-16T00:00:00-08:00\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"nullable\": false,\n      \"enum\": [\n        \"New\",\n        \"Approved\",\n        \"Conditional\",\n        \"Disqualified\",\n        \"Inactive\"\n      ],\n      \"description\": \"Current qualification status of the supplier.\",\n      \"example\": \"Conditional\"\n    },\n    \"review_status\": {\n      \"type\"\
  : \"string\",\n      \"nullable\": false,\n      \"enum\": [\n        \"Pending\",\n        \"Reviewed\",\n        \"N/A\"\n      ],\n      \"description\": \"Review status of the qualification assessment.\",\n      \"example\": \"Reviewed\"\n    },\n    \"frequency\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"nullable\": false,\n      \"minimum\": 1,\n      \"description\": \"Review frequency in months for re-qualification.\",\n      \"example\": 12\n    }\n  },\n  \"required\": [\n    \"date\",\n    \"status\",\n    \"review_status\",\n    \"frequency\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-qualification-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: Qualification
---
