---
description: Filter events using an event pattern. For more information, see <a href="https://docs.aws.amazon.com/eventbridge/latest/userguide/eventbridge-and-event-patterns.html">Events and Event Patterns</a> in the <i>Amazon EventBridge User Guide</i>.
layout: schema
name: Filter
properties_list:
- description: ''
  name: Pattern
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-filter-schema.json
slug: amazon-eventbridge-pipes-filter
source_filename: amazon-eventbridge-pipes-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-filter-schema.json\",\n  \"title\": \"Filter\",\n  \"description\": \"Filter events using an event pattern. For more information, see <a href=\\\"https://docs.aws.amazon.com/eventbridge/latest/userguide/eventbridge-and-event-patterns.html\\\">Events and Event Patterns</a> in the <i>Amazon EventBridge User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Pattern\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventPattern\"\n        },\n        {\n          \"description\": \"The event pattern.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-filter-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: Filter
---
