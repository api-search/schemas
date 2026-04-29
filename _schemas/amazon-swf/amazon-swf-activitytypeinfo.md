---
description: Detailed information about an activity type.
layout: schema
name: ActivityTypeInfo
properties_list:
- description: ''
  name: activityType
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: deprecationDate
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-activitytypeinfo-schema.json
slug: amazon-swf-activitytypeinfo
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"activityType\",\n    \"status\",\n    \"creationDate\"\n  ],\n  \"properties\": {\n    \"activityType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityType\"\n        },\n        {\n          \"description\": \"The <a>ActivityType</a> type structure representing the activity type.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistrationStatus\"\n        },\n        {\n          \"description\": \"The current status of the activity type.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the activity type provided in <a>RegisterActivityType</a>.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time this activity type was created through <a>RegisterActivityType</a>.\"\n        }\n      ]\n    },\n    \"deprecationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"If DEPRECATED, the date and time <a>DeprecateActivityType</a> was called.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Detailed information about an activity type.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ActivityTypeInfo\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-activitytypeinfo-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ActivityTypeInfo
---
