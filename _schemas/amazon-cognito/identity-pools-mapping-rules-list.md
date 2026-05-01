---
description: MappingRulesList schema from Amazon Cognito API
layout: schema
name: MappingRulesList
properties_list: []
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-mapping-rules-list-schema.json
slug: identity-pools-mapping-rules-list
source_filename: identity-pools-mapping-rules-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-mapping-rules-list-schema.json\",\n  \"title\": \"MappingRulesList\",\n  \"description\": \"MappingRulesList schema from Amazon Cognito API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/MappingRule\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 400\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-mapping-rules-list-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: MappingRulesList
---
