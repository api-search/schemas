---
description: SecurityGroups schema from Amazon EventBridge Pipes
layout: schema
name: SecurityGroups
properties_list: []
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-security-groups-schema.json
slug: amazon-eventbridge-pipes-security-groups
source_filename: amazon-eventbridge-pipes-security-groups-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-security-groups-schema.json\",\n  \"title\": \"SecurityGroups\",\n  \"description\": \"SecurityGroups schema from Amazon EventBridge Pipes\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/SecurityGroup\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 5\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-security-groups-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: SecurityGroups
---
