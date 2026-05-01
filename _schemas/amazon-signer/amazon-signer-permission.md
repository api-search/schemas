---
description: A cross-account permission for a signing profile.
layout: schema
name: Permission
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: principal
  type: object
- description: ''
  name: statementId
  type: object
- description: ''
  name: profileVersion
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-permission-schema.json
slug: amazon-signer-permission
source_filename: amazon-signer-permission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-permission-schema.json\",\n  \"title\": \"Permission\",\n  \"description\": \"A cross-account permission for a signing profile.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"An AWS Signer action permitted as part of cross-account permissions.\"\n        }\n      ]\n    },\n    \"principal\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The AWS principal that has been granted a cross-account permission.\"\n        }\n      ]\n    },\n    \"statementId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"A unique identifier\
  \ for a cross-account permission statement.\"\n        }\n      ]\n    },\n    \"profileVersion\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-zA-Z0-9]{10}$\",\n          \"minLength\": 10,\n          \"maxLength\": 10\n        },\n        {\n          \"description\": \"The signing profile version that a permission applies to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-permission-schema.json
tags:
- Code Signing
- IoT
- Lambda
- Security
title: Permission
---
