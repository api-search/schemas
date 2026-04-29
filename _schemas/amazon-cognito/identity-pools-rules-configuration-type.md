---
description: A container for rules.
layout: schema
name: RulesConfigurationType
properties_list:
- description: ''
  name: Rules
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-rules-configuration-type-schema.json
slug: identity-pools-rules-configuration-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-rules-configuration-type-schema.json\",\n  \"title\": \"RulesConfigurationType\",\n  \"description\": \"A container for rules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MappingRulesList\"\n        },\n        {\n          \"description\": \"<p>An array of rules. You can specify up to 25 rules per identity provider.</p> <p>Rules are evaluated in order. The first one to match specifies the role.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Rules\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-rules-configuration-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: RulesConfigurationType
---
