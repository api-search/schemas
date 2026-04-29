---
description: ''
layout: schema
name: Education
properties_list:
- description: ''
  name: school
  type: string
- description: ''
  name: educationDegree
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-education-schema.json
slug: zoominfo-education
source_filename: zoominfo-education-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"school\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"educationDegree\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"degree\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"areaOfStudy\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"degree\",\n        \"areaOfStudy\"\n      ]\n    }\n  },\n  \"required\": [\n    \"school\",\n    \"educationDegree\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Education\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-education-schema.json
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
title: Education
---
