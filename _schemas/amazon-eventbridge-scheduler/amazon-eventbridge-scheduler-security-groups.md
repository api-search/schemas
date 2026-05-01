---
description: SecurityGroups schema from Amazon EventBridge Scheduler
layout: schema
name: SecurityGroups
properties_list: []
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-security-groups-schema.json
slug: amazon-eventbridge-scheduler-security-groups
source_filename: amazon-eventbridge-scheduler-security-groups-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-security-groups-schema.json\",\n  \"title\": \"SecurityGroups\",\n  \"description\": \"SecurityGroups schema from Amazon EventBridge Scheduler\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/SecurityGroup\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 5\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-security-groups-schema.json
tags:
- Amazon Web Services
- Cron
- Event-Driven
- Scheduling
- Serverless
title: SecurityGroups
---
