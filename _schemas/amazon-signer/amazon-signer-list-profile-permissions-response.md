---
description: ListProfilePermissionsResponse schema from AWS Signer API
layout: schema
name: ListProfilePermissionsResponse
properties_list:
- description: ''
  name: revisionId
  type: object
- description: ''
  name: policySizeBytes
  type: object
- description: ''
  name: permissions
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-list-profile-permissions-response-schema.json
slug: amazon-signer-list-profile-permissions-response
source_filename: amazon-signer-list-profile-permissions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-list-profile-permissions-response-schema.json\",\n  \"title\": \"ListProfilePermissionsResponse\",\n  \"description\": \"ListProfilePermissionsResponse schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The identifier for the current revision of profile permissions.\"\n        }\n      ]\n    },\n    \"policySizeBytes\": {\n      \"allOf\": [\n        {\n          \"type\": \"integer\"\n        },\n        {\n          \"description\": \"Total size of the policy associated with the Signing Profile in bytes.\"\n        }\n      ]\n    },\n    \"permissions\": {\n      \"allOf\": [\n        {\n          \"type\": \"array\",\n     \
  \     \"items\": {\n            \"$ref\": \"#/components/schemas/Permission\"\n          }\n        },\n        {\n          \"description\": \"List of permissions associated with the Signing Profile.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"String for specifying the next set of paginated results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-list-profile-permissions-response-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: ListProfilePermissionsResponse
---
