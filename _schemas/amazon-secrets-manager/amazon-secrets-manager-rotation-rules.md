---
description: RotationRules schema from Amazon Secrets Manager API
layout: schema
name: RotationRules
properties_list:
- description: The number of days between automatic scheduled rotations.
  name: AutomaticallyAfterDays
  type: integer
- description: The length of the rotation window in hours.
  name: Duration
  type: string
- description: A cron or rate expression that defines the schedule for rotation.
  name: ScheduleExpression
  type: string
provider_name: Amazon Secrets Manager
provider_slug: amazon-secrets-manager
schema_file: json-schema/amazon-secrets-manager-rotation-rules-schema.json
slug: amazon-secrets-manager-rotation-rules
source_filename: amazon-secrets-manager-rotation-rules-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/json-schema/amazon-secrets-manager-rotation-rules-schema.json\",\n  \"title\": \"RotationRules\",\n  \"description\": \"RotationRules schema from Amazon Secrets Manager API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutomaticallyAfterDays\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of days between automatic scheduled rotations.\"\n    },\n    \"Duration\": {\n      \"type\": \"string\",\n      \"description\": \"The length of the rotation window in hours.\"\n    },\n    \"ScheduleExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A cron or rate expression that defines the schedule for rotation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/json-schema/amazon-secrets-manager-rotation-rules-schema.json
tags:
- Configuration
- Credentials
- Rotation
- Secrets
- Security
title: RotationRules
---
