---
description: Contains summary information about hours of operation for a contact center.
layout: schema
name: HoursOfOperationSummary
properties_list:
- description: The identifier of the hours of operation.
  name: Id
  type: string
- description: The Amazon Resource Name (ARN) of the hours of operation.
  name: Arn
  type: string
- description: The name of the hours of operation.
  name: Name
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/hours-of-operation-summary-schema.json
slug: hours-of-operation-summary
source_filename: hours-of-operation-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/hours-of-operation-summary-schema.json\",\n  \"title\": \"HoursOfOperationSummary\",\n  \"description\": \"Contains summary information about hours of operation for a contact center.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the hours of operation.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-66666EXAMPLE\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the hours of operation.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the hours of operation.\",\n      \"example\": \"Business Hours\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/hours-of-operation-summary-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: HoursOfOperationSummary
---
