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
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-string-attribute-constraints-type-schema.json
slug: cognito-idp-string-attribute-constraints-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"MinLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The minimum length.\"\n        }\n      ]\n    },\n    \"MaxLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The maximum length.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The constraints associated with a string attribute.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-string-attribute-constraints-type-schema.json\",\n  \"title\": \"StringAttributeConstraintsType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-string-attribute-constraints-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: StringAttributeConstraintsType
---
