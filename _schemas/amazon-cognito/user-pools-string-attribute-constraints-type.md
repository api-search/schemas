---
description: The constraints associated with a string attribute.
layout: schema
name: StringAttributeConstraintsType
properties_list:
- description: ''
  name: MinLength
  type: object
- description: ''
  name: MaxLength
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-string-attribute-constraints-type-schema.json
slug: user-pools-string-attribute-constraints-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-string-attribute-constraints-type-schema.json\",\n  \"title\": \"StringAttributeConstraintsType\",\n  \"description\": \"The constraints associated with a string attribute.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MinLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The minimum length.\"\n        }\n      ]\n    },\n    \"MaxLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The maximum length.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-string-attribute-constraints-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: StringAttributeConstraintsType
---
