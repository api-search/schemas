---
description: CapacityProviderStrategy schema from Amazon EventBridge Scheduler
layout: schema
name: CapacityProviderStrategy
properties_list: []
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-capacity-provider-strategy-schema.json
slug: amazon-eventbridge-scheduler-capacity-provider-strategy
source_filename: amazon-eventbridge-scheduler-capacity-provider-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-capacity-provider-strategy-schema.json\",\n  \"title\": \"CapacityProviderStrategy\",\n  \"description\": \"CapacityProviderStrategy schema from Amazon EventBridge Scheduler\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/CapacityProviderStrategyItem\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 6\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-capacity-provider-strategy-schema.json
tags:
- Amazon Web Services
- Cron
- Event-Driven
- Scheduling
- Serverless
title: CapacityProviderStrategy
---
