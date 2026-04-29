---
description: Contains information about the hours of operation.
layout: schema
name: HoursOfOperationConfig
properties_list:
- description: The day that the hours of operation applies to.
  name: Day
  type: string
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/hours-of-operation-config-schema.json
slug: hours-of-operation-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/hours-of-operation-config-schema.json\",\n  \"title\": \"HoursOfOperationConfig\",\n  \"description\": \"Contains information about the hours of operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Day\": {\n      \"type\": \"string\",\n      \"description\": \"The day that the hours of operation applies to.\",\n      \"enum\": [\n        \"SUNDAY\",\n        \"MONDAY\",\n        \"TUESDAY\",\n        \"WEDNESDAY\",\n        \"THURSDAY\",\n        \"FRIDAY\",\n        \"SATURDAY\"\n      ],\n      \"example\": \"MONDAY\"\n    },\n    \"StartTime\": {\n      \"$ref\": \"#/components/schemas/HoursOfOperationTimeSlice\"\n    },\n    \"EndTime\": {\n      \"$ref\": \"#/components/schemas/HoursOfOperationTimeSlice\"\n    }\n  },\n  \"required\": [\n    \"Day\",\n    \"StartTime\",\n    \"EndTime\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/hours-of-operation-config-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: HoursOfOperationConfig
---
