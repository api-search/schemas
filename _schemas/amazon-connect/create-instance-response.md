---
description: CreateInstanceResponse schema from Amazon Connect Service API
layout: schema
name: CreateInstanceResponse
properties_list:
- description: The identifier for the instance.
  name: Id
  type: string
- description: The Amazon Resource Name (ARN) of the instance.
  name: Arn
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/create-instance-response-schema.json
slug: create-instance-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-instance-response-schema.json\",\n  \"title\": \"CreateInstanceResponse\",\n  \"description\": \"CreateInstanceResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the instance.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-11111EXAMPLE\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the instance.\",\n      \"example\": \"arn:aws:connect:us-east-1:123456789012:instance/a1b2c3d4-5678-90ab-cdef-11111EXAMPLE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-instance-response-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: CreateInstanceResponse
---
