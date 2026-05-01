---
description: ''
layout: schema
name: DeprecateActivityTypeInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: activityType
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-deprecateactivitytypeinput-schema.json
slug: amazon-swf-deprecateactivitytypeinput
source_filename: amazon-swf-deprecateactivitytypeinput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"activityType\"\n  ],\n  \"title\": \"DeprecateActivityTypeInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain in which the activity type is registered.\"\n        }\n      ]\n    },\n    \"activityType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityType\"\n        },\n        {\n          \"description\": \"The activity type to deprecate.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-deprecateactivitytypeinput-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: DeprecateActivityTypeInput
---
