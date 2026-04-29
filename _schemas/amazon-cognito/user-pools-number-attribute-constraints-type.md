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
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-number-attribute-constraints-type-schema.json
slug: user-pools-number-attribute-constraints-type
source_filename: user-pools-number-attribute-constraints-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-number-attribute-constraints-type-schema.json\",\n  \"title\": \"NumberAttributeConstraintsType\",\n  \"description\": \"The minimum and maximum values of an attribute that is of the number data type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MinValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The minimum value of an attribute that is of the number data type.\"\n        }\n      ]\n    },\n    \"MaxValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The maximum value of an attribute that is of the number data type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-number-attribute-constraints-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: NumberAttributeConstraintsType
---
