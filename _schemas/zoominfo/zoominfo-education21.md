---
description: ''
layout: schema
name: Education21
properties_list:
- description: ''
  name: school
  type: string
- description: ''
  name: educationDegree
  type: object
- description: ''
  name: graduationDate
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-education21-schema.json
slug: zoominfo-education21
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"school\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"educationDegree\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"degree\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"areaOfStudy\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"degree\",\n        \"areaOfStudy\"\n      ]\n    },\n    \"graduationDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Education21\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-education21-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: Education21
---
