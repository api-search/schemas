---
description: The start or end time of an hours of operation.
layout: schema
name: HoursOfOperationTimeSlice
properties_list:
- description: The hours.
  name: Hours
  type: integer
- description: The minutes.
  name: Minutes
  type: integer
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/hours-of-operation-time-slice-schema.json
slug: hours-of-operation-time-slice
source_filename: hours-of-operation-time-slice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/hours-of-operation-time-slice-schema.json\",\n  \"title\": \"HoursOfOperationTimeSlice\",\n  \"description\": \"The start or end time of an hours of operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Hours\": {\n      \"type\": \"integer\",\n      \"description\": \"The hours.\",\n      \"minimum\": 0,\n      \"maximum\": 23,\n      \"example\": 9\n    },\n    \"Minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"The minutes.\",\n      \"minimum\": 0,\n      \"maximum\": 59,\n      \"example\": 0\n    }\n  },\n  \"required\": [\n    \"Hours\",\n    \"Minutes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/hours-of-operation-time-slice-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: HoursOfOperationTimeSlice
---
