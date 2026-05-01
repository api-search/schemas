---
description: ''
layout: schema
name: UndeprecateActivityTypeInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: activityType
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-undeprecateactivitytypeinput-schema.json
slug: amazon-swf-undeprecateactivitytypeinput
source_filename: amazon-swf-undeprecateactivitytypeinput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"activityType\"\n  ],\n  \"title\": \"UndeprecateActivityTypeInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain of the deprecated activity type.\"\n        }\n      ]\n    },\n    \"activityType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityType\"\n        },\n        {\n          \"description\": \"The activity type to undeprecate.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-undeprecateactivitytypeinput-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: UndeprecateActivityTypeInput
---
