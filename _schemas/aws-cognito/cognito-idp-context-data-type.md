---
description: Contextual user data type used for evaluating the risk of an unexpected event by Amazon Cognito advanced security.
layout: schema
name: ContextDataType
properties_list:
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: ServerName
  type: object
- description: ''
  name: ServerPath
  type: object
- description: ''
  name: HttpHeaders
  type: object
- description: ''
  name: EncodedData
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-context-data-type-schema.json
slug: cognito-idp-context-data-type
source_filename: cognito-idp-context-data-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The source IP address of your user's device.\"\n        }\n      ]\n    },\n    \"ServerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"Your server endpoint where this API is invoked.\"\n        }\n      ]\n    },\n    \"ServerPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"Your server path where this API is invoked.\"\n        }\n      ]\n    },\n    \"HttpHeaders\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpHeaderList\"\n        },\n        {\n          \"description\": \"HttpHeaders received on your server in same order.\"\n\
  \        }\n      ]\n    },\n    \"EncodedData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"Encoded device-fingerprint details that your app collected with the Amazon Cognito context data collection library. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pool-settings-adaptive-authentication.html#user-pool-settings-adaptive-authentication-device-fingerprint\\\">Adding user device and session data to API requests</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IpAddress\",\n    \"ServerName\",\n    \"ServerPath\",\n    \"HttpHeaders\"\n  ],\n  \"description\": \"Contextual user data type used for evaluating the risk of an unexpected event by Amazon Cognito advanced security.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-context-data-type-schema.json\"\
  ,\n  \"title\": \"ContextDataType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-context-data-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ContextDataType
---
