---
description: A rule that maps a claim name, a claim value, and a match type to a role ARN.
layout: schema
name: MappingRule
properties_list:
- description: ''
  name: Claim
  type: object
- description: ''
  name: MatchType
  type: object
- description: ''
  name: Value
  type: object
- description: ''
  name: RoleARN
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-mapping-rule-schema.json
slug: identity-pools-mapping-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-mapping-rule-schema.json\",\n  \"title\": \"MappingRule\",\n  \"description\": \"A rule that maps a claim name, a claim value, and a match type to a role ARN.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Claim\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClaimName\"\n        },\n        {\n          \"description\": \"The claim name that must be present in the token, for example, \\\"isAdmin\\\" or \\\"paid\\\".\"\n        }\n      ]\n    },\n    \"MatchType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MappingRuleMatchType\"\n        },\n        {\n          \"description\": \"The match condition that specifies how closely the claim value in the IdP token must match <code>Value</code>.\"\n        }\n      ]\n\
  \    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClaimValue\"\n        },\n        {\n          \"description\": \"A brief string that the claim must match, for example, \\\"paid\\\" or \\\"yes\\\".\"\n        }\n      ]\n    },\n    \"RoleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARNString\"\n        },\n        {\n          \"description\": \"The role ARN.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Claim\",\n    \"MatchType\",\n    \"Value\",\n    \"RoleARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-mapping-rule-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: MappingRule
---
