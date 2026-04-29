---
description: Specifies the event feedback type.
layout: schema
name: EventFeedbackType
properties_list:
- description: ''
  name: FeedbackValue
  type: object
- description: ''
  name: Provider
  type: object
- description: ''
  name: FeedbackDate
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-event-feedback-type-schema.json
slug: cognito-idp-event-feedback-type
source_filename: cognito-idp-event-feedback-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"FeedbackValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FeedbackValueType\"\n        },\n        {\n          \"description\": \"The event feedback value.\"\n        }\n      ]\n    },\n    \"Provider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The provider.\"\n        }\n      ]\n    },\n    \"FeedbackDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The event feedback date.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FeedbackValue\",\n    \"Provider\"\n  ],\n  \"description\": \"Specifies the event feedback type.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-event-feedback-type-schema.json\"\
  ,\n  \"title\": \"EventFeedbackType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-event-feedback-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: EventFeedbackType
---
