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
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-event-context-data-type-schema.json
slug: cognito-idp-event-context-data-type
source_filename: cognito-idp-event-context-data-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The source IP address of your user's device.\"\n        }\n      ]\n    },\n    \"DeviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The user's device name.\"\n        }\n      ]\n    },\n    \"Timezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The user's time zone.\"\n        }\n      ]\n    },\n    \"City\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The user's city.\"\n        }\n      ]\n    },\n    \"Country\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The user's country.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Specifies the user context data captured at the time of an event request.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-event-context-data-type-schema.json\",\n  \"title\": \"EventContextDataType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-event-context-data-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: EventContextDataType
---
