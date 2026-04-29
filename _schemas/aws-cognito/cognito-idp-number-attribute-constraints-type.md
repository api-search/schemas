---
description: The minimum and maximum values of an attribute that is of the number data type.
layout: schema
name: NumberAttributeConstraintsType
properties_list:
- description: ''
  name: MinValue
  type: object
- description: ''
  name: MaxValue
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-number-attribute-constraints-type-schema.json
slug: cognito-idp-number-attribute-constraints-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"MinValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The minimum value of an attribute that is of the number data type.\"\n        }\n      ]\n    },\n    \"MaxValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The maximum value of an attribute that is of the number data type.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The minimum and maximum values of an attribute that is of the number data type.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-number-attribute-constraints-type-schema.json\",\n  \"title\": \"NumberAttributeConstraintsType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-number-attribute-constraints-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: NumberAttributeConstraintsType
---
