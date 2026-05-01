---
description: MappingRulesList schema from Amazon Cognito
layout: schema
name: MappingRulesList
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-mapping-rules-list-schema.json
slug: cognito-identity-mapping-rules-list
source_filename: cognito-identity-mapping-rules-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Claim\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ClaimName\"\n          },\n          {\n            \"description\": \"The claim name that must be present in the token, for example, \\\"isAdmin\\\" or \\\"paid\\\".\"\n          }\n        ]\n      },\n      \"MatchType\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/MappingRuleMatchType\"\n          },\n          {\n            \"description\": \"The match condition that specifies how closely the claim value in the IdP token must match <code>Value</code>.\"\n          }\n        ]\n      },\n      \"Value\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ClaimValue\"\n          },\n          {\n            \"description\": \"A brief string that the claim must match, for example, \\\"paid\\\" or \\\"yes\\\".\"\
  \n          }\n        ]\n      },\n      \"RoleARN\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ARNString\"\n          },\n          {\n            \"description\": \"The role ARN.\"\n          }\n        ]\n      }\n    },\n    \"required\": [\n      \"Claim\",\n      \"MatchType\",\n      \"Value\",\n      \"RoleARN\"\n    ],\n    \"description\": \"A rule that maps a claim name, a claim value, and a match type to a role ARN.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-mapping-rules-list-schema.json\",\n  \"title\": \"MappingRulesList\",\n  \"description\": \"MappingRulesList schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-mapping-rules-list-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: MappingRulesList
---
