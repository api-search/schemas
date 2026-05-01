---
description: A render farm in Amazon Deadline Cloud that contains queues, fleets, and jobs.
layout: schema
name: Farm
properties_list:
- description: The unique identifier of the render farm
  name: farmId
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: description
  type: string
- description: The ARN of the KMS key. This ARN uniquely identifies the key.
  name: kmsKeyArn
  type: string
- description: ''
  name: createdAt
  type: string
provider_name: Amazon Deadline Cloud
provider_slug: amazon-deadline-cloud
schema_file: json-schema/farm-schema.json
slug: farm
source_filename: farm-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deadline-cloud/json-schema/farm-schema.json\",\n  \"title\": \"Farm\",\n  \"description\": \"A render farm in Amazon Deadline Cloud that contains queues, fleets, and jobs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"farmId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the render farm\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"kmsKeyArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the KMS key. This ARN uniquely identifies the key.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/json-schema/farm-schema.json
tags:
- Compute
- Media
- Rendering
- Visual Effects
title: Farm
---
