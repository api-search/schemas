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
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-event-risk-type-schema.json
slug: cognito-idp-event-risk-type
source_filename: cognito-idp-event-risk-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"RiskDecision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RiskDecisionType\"\n        },\n        {\n          \"description\": \"The risk decision.\"\n        }\n      ]\n    },\n    \"RiskLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RiskLevelType\"\n        },\n        {\n          \"description\": \"The risk level.\"\n        }\n      ]\n    },\n    \"CompromisedCredentialsDetected\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrappedBooleanType\"\n        },\n        {\n          \"description\": \"Indicates whether compromised credentials were detected during an authentication event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The event risk type.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-event-risk-type-schema.json\"\
  ,\n  \"title\": \"EventRiskType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-event-risk-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: EventRiskType
---
