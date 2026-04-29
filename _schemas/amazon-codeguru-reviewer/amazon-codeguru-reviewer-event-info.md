---
description: Information about an event. The event might be a push, pull request, scheduled request, or another type of event.
layout: schema
name: EventInfo
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: State
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-event-info-schema.json
slug: amazon-codeguru-reviewer-event-info
source_filename: amazon-codeguru-reviewer-event-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-event-info-schema.json\",\n  \"title\": \"EventInfo\",\n  \"description\": \"Information about an event. The event might be a push, pull request, scheduled request, or another type of event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventName\"\n        },\n        {\n          \"description\": \"The name of the event. The possible names are <code>pull_request</code>, <code>workflow_dispatch</code>, <code>schedule</code>, and <code>push</code> \"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventState\"\n        },\n        {\n          \"description\": \"The state of an event. The state might be\
  \ open, closed, or another state.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-event-info-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: EventInfo
---
