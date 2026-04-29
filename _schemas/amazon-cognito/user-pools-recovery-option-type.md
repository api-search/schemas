---
description: A map containing a priority as a key, and recovery method name as a value.
layout: schema
name: RecoveryOptionType
properties_list:
- description: ''
  name: Priority
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-recovery-option-type-schema.json
slug: user-pools-recovery-option-type
source_filename: user-pools-recovery-option-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-recovery-option-type-schema.json\",\n  \"title\": \"RecoveryOptionType\",\n  \"description\": \"A map containing a priority as a key, and recovery method name as a value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PriorityType\"\n        },\n        {\n          \"description\": \"A positive integer specifying priority of a method with 1 being the highest priority.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecoveryOptionNameType\"\n        },\n        {\n          \"description\": \"The recovery method for a user.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Priority\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-recovery-option-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: RecoveryOptionType
---
