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
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-event-feedback-type-schema.json
slug: user-pools-event-feedback-type
source_filename: user-pools-event-feedback-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-event-feedback-type-schema.json\",\n  \"title\": \"EventFeedbackType\",\n  \"description\": \"Specifies the event feedback type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FeedbackValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FeedbackValueType\"\n        },\n        {\n          \"description\": \"The authentication event feedback value. When you provide a <code>FeedbackValue</code> value of <code>valid</code>, you tell Amazon Cognito that you trust a user session where Amazon Cognito has evaluated some level of risk. When you provide a <code>FeedbackValue</code> value of <code>invalid</code>, you tell Amazon Cognito that you don't trust a user session, or you don't believe that Amazon Cognito evaluated a high-enough risk level.\"\n       \
  \ }\n      ]\n    },\n    \"Provider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The provider.\"\n        }\n      ]\n    },\n    \"FeedbackDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The event feedback date.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FeedbackValue\",\n    \"Provider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-event-feedback-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: EventFeedbackType
---
