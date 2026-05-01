---
description: AdminUpdateAuthEventFeedbackRequest schema from Amazon Cognito
layout: schema
name: AdminUpdateAuthEventFeedbackRequest
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
  name: FeedbackValue
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-admin-update-auth-event-feedback-request-schema.json
slug: cognito-idp-admin-update-auth-event-feedback-request
source_filename: cognito-idp-admin-update-auth-event-feedback-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\": \"The user pool username.\"\n        }\n      ]\n    },\n    \"EventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventIdType\"\n        },\n        {\n          \"description\": \"The authentication event ID.\"\n        }\n      ]\n    },\n    \"FeedbackValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FeedbackValueType\"\n        },\n        {\n          \"description\": \"The authentication event feedback value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\"\
  ,\n    \"Username\",\n    \"EventId\",\n    \"FeedbackValue\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-update-auth-event-feedback-request-schema.json\",\n  \"title\": \"AdminUpdateAuthEventFeedbackRequest\",\n  \"description\": \"AdminUpdateAuthEventFeedbackRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-update-auth-event-feedback-request-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AdminUpdateAuthEventFeedbackRequest
---
