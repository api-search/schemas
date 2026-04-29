---
description: Contextual data, such as the user's device fingerprint, IP address, or location, used for evaluating the risk of an unexpected event by Amazon Cognito advanced security.
layout: schema
name: UserContextDataType
properties_list:
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: EncodedData
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-user-context-data-type-schema.json
slug: cognito-idp-user-context-data-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The source IP address of your user's device.\"\n        }\n      ]\n    },\n    \"EncodedData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"Encoded device-fingerprint details that your app collected with the Amazon Cognito context data collection library. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pool-settings-adaptive-authentication.html#user-pool-settings-adaptive-authentication-device-fingerprint\\\">Adding user device and session data to API requests</a>.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contextual data, such as the user's device fingerprint, IP address, or location, used for\
  \ evaluating the risk of an unexpected event by Amazon Cognito advanced security.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-user-context-data-type-schema.json\",\n  \"title\": \"UserContextDataType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-user-context-data-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UserContextDataType
---
