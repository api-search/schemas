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
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-auth-event-type-schema.json
slug: user-pools-auth-event-type
source_filename: user-pools-auth-event-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-auth-event-type-schema.json\",\n  \"title\": \"AuthEventType\",\n  \"description\": \"The authentication event type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The event ID.\"\n        }\n      ]\n    },\n    \"EventType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventType\"\n        },\n        {\n          \"description\": \"The event type.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date and time, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\
  \">ISO 8601</a> format, when the item was created.\"\n        }\n      ]\n    },\n    \"EventResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventResponseType\"\n        },\n        {\n          \"description\": \"The event response.\"\n        }\n      ]\n    },\n    \"EventRisk\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventRiskType\"\n        },\n        {\n          \"description\": \"The event risk.\"\n        }\n      ]\n    },\n    \"ChallengeResponses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChallengeResponseListType\"\n        },\n        {\n          \"description\": \"The challenge responses.\"\n        }\n      ]\n    },\n    \"EventContextData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventContextDataType\"\n        },\n        {\n          \"description\": \"The user context data captured at the time of an event request.\
  \ This value provides additional information about the client from which event the request is received.\"\n        }\n      ]\n    },\n    \"EventFeedback\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventFeedbackType\"\n        },\n        {\n          \"description\": \"A flag specifying the user feedback captured at the time of an event request is good or bad. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-auth-event-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: AuthEventType
---
