---
description: The event risk type.
layout: schema
name: EventRiskType
properties_list:
- description: ''
  name: RiskDecision
  type: object
- description: ''
  name: RiskLevel
  type: object
- description: ''
  name: CompromisedCredentialsDetected
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-event-risk-type-schema.json
slug: user-pools-event-risk-type
source_filename: user-pools-event-risk-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-event-risk-type-schema.json\",\n  \"title\": \"EventRiskType\",\n  \"description\": \"The event risk type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RiskDecision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RiskDecisionType\"\n        },\n        {\n          \"description\": \"The risk decision.\"\n        }\n      ]\n    },\n    \"RiskLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RiskLevelType\"\n        },\n        {\n          \"description\": \"The risk level.\"\n        }\n      ]\n    },\n    \"CompromisedCredentialsDetected\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrappedBooleanType\"\n        },\n        {\n          \"description\": \"Indicates whether compromised\
  \ credentials were detected during an authentication event.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-event-risk-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: EventRiskType
---
