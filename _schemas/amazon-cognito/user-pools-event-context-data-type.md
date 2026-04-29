---
description: Specifies the user context data captured at the time of an event request.
layout: schema
name: EventContextDataType
properties_list:
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: DeviceName
  type: object
- description: ''
  name: Timezone
  type: object
- description: ''
  name: City
  type: object
- description: ''
  name: Country
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-event-context-data-type-schema.json
slug: user-pools-event-context-data-type
source_filename: user-pools-event-context-data-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-event-context-data-type-schema.json\",\n  \"title\": \"EventContextDataType\",\n  \"description\": \"Specifies the user context data captured at the time of an event request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The source IP address of your user's device.\"\n        }\n      ]\n    },\n    \"DeviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The user's device name.\"\n        }\n      ]\n    },\n    \"Timezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n\
  \        {\n          \"description\": \"The user's time zone.\"\n        }\n      ]\n    },\n    \"City\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The user's city.\"\n        }\n      ]\n    },\n    \"Country\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The user's country.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-event-context-data-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: EventContextDataType
---
