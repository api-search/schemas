---
description: A compute fleet in a render farm providing worker capacity for jobs.
layout: schema
name: Fleet
properties_list:
- description: The unique identifier of the fleet
  name: fleetId
  type: string
- description: ''
  name: farmId
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: workerCount
  type: integer
- description: The ARN of the IAM role for the fleet
  name: roleArn
  type: string
- description: ''
  name: createdAt
  type: string
provider_name: Amazon Deadline Cloud
provider_slug: amazon-deadline-cloud
schema_file: json-schema/fleet-schema.json
slug: fleet
source_filename: fleet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deadline-cloud/json-schema/fleet-schema.json\",\n  \"title\": \"Fleet\",\n  \"description\": \"A compute fleet in a render farm providing worker capacity for jobs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fleetId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the fleet\"\n    },\n    \"farmId\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"workerCount\": {\n      \"type\": \"integer\"\n    },\n    \"roleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the IAM role for the fleet\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/json-schema/fleet-schema.json
tags:
- Compute
- Media
- Rendering
- Visual Effects
title: Fleet
---
