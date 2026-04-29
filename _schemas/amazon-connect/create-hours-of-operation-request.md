---
description: CreateHoursOfOperationRequest schema from Amazon Connect Service API
layout: schema
name: CreateHoursOfOperationRequest
properties_list:
- description: The name of the hours of operation.
  name: Name
  type: string
- description: The description of the hours of operation.
  name: Description
  type: string
- description: The time zone of the hours of operation.
  name: TimeZone
  type: string
- description: ''
  name: Config
  type: array
- description: ''
  name: Tags
  type: object
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/create-hours-of-operation-request-schema.json
slug: create-hours-of-operation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-hours-of-operation-request-schema.json\",\n  \"title\": \"CreateHoursOfOperationRequest\",\n  \"description\": \"CreateHoursOfOperationRequest schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the hours of operation.\",\n      \"example\": \"Business Hours\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the hours of operation.\"\n    },\n    \"TimeZone\": {\n      \"type\": \"string\",\n      \"description\": \"The time zone of the hours of operation.\",\n      \"example\": \"America/New_York\"\n    },\n    \"Config\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/HoursOfOperationConfig\"\
  \n      }\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"Config\",\n    \"Name\",\n    \"TimeZone\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-hours-of-operation-request-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: CreateHoursOfOperationRequest
---
