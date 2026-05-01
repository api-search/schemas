---
description: A container for rules.
layout: schema
name: RulesConfigurationType
properties_list:
- description: ''
  name: Rules
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-rules-configuration-type-schema.json
slug: cognito-identity-rules-configuration-type
source_filename: cognito-identity-rules-configuration-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MappingRulesList\"\n        },\n        {\n          \"description\": \"<p>An array of rules. You can specify up to 25 rules per identity provider.</p> <p>Rules are evaluated in order. The first one to match specifies the role.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Rules\"\n  ],\n  \"description\": \"A container for rules.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-rules-configuration-type-schema.json\",\n  \"title\": \"RulesConfigurationType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-rules-configuration-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: RulesConfigurationType
---
