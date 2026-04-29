---
description: The authentication event type.
layout: schema
name: AuthEventType
properties_list:
- description: ''
  name: EventId
  type: object
- description: ''
  name: EventType
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: EventResponse
  type: object
- description: ''
  name: EventRisk
  type: object
- description: ''
  name: ChallengeResponses
  type: object
- description: ''
  name: EventContextData
  type: object
- description: ''
  name: EventFeedback
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-auth-event-type-schema.json
slug: cognito-idp-auth-event-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"EventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The event ID.\"\n        }\n      ]\n    },\n    \"EventType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventType\"\n        },\n        {\n          \"description\": \"The event type.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The creation date\"\n        }\n      ]\n    },\n    \"EventResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventResponseType\"\n        },\n        {\n          \"description\": \"The event response.\"\n        }\n      ]\n    },\n    \"EventRisk\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventRiskType\"\
  \n        },\n        {\n          \"description\": \"The event risk.\"\n        }\n      ]\n    },\n    \"ChallengeResponses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChallengeResponseListType\"\n        },\n        {\n          \"description\": \"The challenge responses.\"\n        }\n      ]\n    },\n    \"EventContextData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventContextDataType\"\n        },\n        {\n          \"description\": \"The user context data captured at the time of an event request. This value provides additional information about the client from which event the request is received.\"\n        }\n      ]\n    },\n    \"EventFeedback\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventFeedbackType\"\n        },\n        {\n          \"description\": \"A flag specifying the user feedback captured at the time of an event request is good or bad. \"\n        }\n\
  \      ]\n    }\n  },\n  \"description\": \"The authentication event type.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-auth-event-type-schema.json\",\n  \"title\": \"AuthEventType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-auth-event-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AuthEventType
---
