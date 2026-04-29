---
description: Specifies whether the attribute is standard or custom.
layout: schema
name: AttributeType
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-attribute-type-schema.json
slug: cognito-idp-attribute-type
source_filename: cognito-idp-attribute-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeNameType\"\n        },\n        {\n          \"description\": \"The name of the attribute.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeValueType\"\n        },\n        {\n          \"description\": \"The value of the attribute.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ],\n  \"description\": \"Specifies whether the attribute is standard or custom.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-attribute-type-schema.json\",\n  \"title\": \"AttributeType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-attribute-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AttributeType
---
