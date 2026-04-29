---
description: PlacementConstraints schema from Amazon EventBridge Scheduler
layout: schema
name: PlacementConstraints
properties_list: []
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-placement-constraints-schema.json
slug: amazon-eventbridge-scheduler-placement-constraints
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-placement-constraints-schema.json\",\n  \"title\": \"PlacementConstraints\",\n  \"description\": \"PlacementConstraints schema from Amazon EventBridge Scheduler\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/PlacementConstraint\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 10\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-placement-constraints-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: PlacementConstraints
---
