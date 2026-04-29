---
description: Configuration for mitigation actions and notification for different levels of risk detected for a potential account takeover.
layout: schema
name: AccountTakeoverRiskConfigurationType
properties_list:
- description: ''
  name: NotifyConfiguration
  type: object
- description: ''
  name: Actions
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-account-takeover-risk-configuration-type-schema.json
slug: user-pools-account-takeover-risk-configuration-type
source_filename: user-pools-account-takeover-risk-configuration-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-account-takeover-risk-configuration-type-schema.json\",\n  \"title\": \"AccountTakeoverRiskConfigurationType\",\n  \"description\": \"Configuration for mitigation actions and notification for different levels of risk detected for a potential account takeover.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NotifyConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotifyConfigurationType\"\n        },\n        {\n          \"description\": \"The notify configuration used to construct email notifications.\"\n        }\n      ]\n    },\n    \"Actions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountTakeoverActionsType\"\n        },\n        {\n          \"description\": \"Account takeover risk configuration actions.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Actions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-account-takeover-risk-configuration-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: AccountTakeoverRiskConfigurationType
---
