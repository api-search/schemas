---
description: Represents the request to add custom attributes.
layout: schema
name: AddCustomAttributesRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: CustomAttributes
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-add-custom-attributes-request-schema.json
slug: user-pools-add-custom-attributes-request
source_filename: user-pools-add-custom-attributes-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-add-custom-attributes-request-schema.json\",\n  \"title\": \"AddCustomAttributesRequest\",\n  \"description\": \"Represents the request to add custom attributes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool where you want to add custom attributes.\"\n        }\n      ]\n    },\n    \"CustomAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomAttributesListType\"\n        },\n        {\n          \"description\": \"An array of custom attributes, such as Mutable and Name.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n\
  \    \"CustomAttributes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-add-custom-attributes-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: AddCustomAttributesRequest
---
