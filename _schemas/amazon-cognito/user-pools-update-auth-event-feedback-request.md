---
description: UpdateAuthEventFeedbackRequest schema from Amazon Cognito API
layout: schema
name: UpdateAuthEventFeedbackRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: Username
  type: object
- description: ''
  name: EventId
  type: object
- description: ''
  name: FeedbackToken
  type: object
- description: ''
  name: FeedbackValue
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-update-auth-event-feedback-request-schema.json
slug: user-pools-update-auth-event-feedback-request
source_filename: user-pools-update-auth-event-feedback-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-auth-event-feedback-request-schema.json\",\n  \"title\": \"UpdateAuthEventFeedbackRequest\",\n  \"description\": \"UpdateAuthEventFeedbackRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\": \"The user pool username.\"\n        }\n      ]\n    },\n    \"EventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventIdType\"\n        },\n        {\n  \
  \        \"description\": \"The event ID.\"\n        }\n      ]\n    },\n    \"FeedbackToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"The feedback token.\"\n        }\n      ]\n    },\n    \"FeedbackValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FeedbackValueType\"\n        },\n        {\n          \"description\": \"The authentication event feedback value. When you provide a <code>FeedbackValue</code> value of <code>valid</code>, you tell Amazon Cognito that you trust a user session where Amazon Cognito has evaluated some level of risk. When you provide a <code>FeedbackValue</code> value of <code>invalid</code>, you tell Amazon Cognito that you don't trust a user session, or you don't believe that Amazon Cognito evaluated a high-enough risk level.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"Username\"\
  ,\n    \"EventId\",\n    \"FeedbackToken\",\n    \"FeedbackValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-auth-event-feedback-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UpdateAuthEventFeedbackRequest
---
