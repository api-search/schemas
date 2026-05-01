---
description: AddProfilePermissionRequest schema from AWS Signer API
layout: schema
name: AddProfilePermissionRequest
properties_list:
- description: ''
  name: profileVersion
  type: object
- description: ''
  name: action
  type: object
- description: ''
  name: principal
  type: object
- description: ''
  name: revisionId
  type: object
- description: ''
  name: statementId
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-add-profile-permission-request-schema.json
slug: amazon-signer-add-profile-permission-request
source_filename: amazon-signer-add-profile-permission-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-add-profile-permission-request-schema.json\",\n  \"title\": \"AddProfilePermissionRequest\",\n  \"description\": \"AddProfilePermissionRequest schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profileVersion\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-zA-Z0-9]{10}$\",\n          \"minLength\": 10,\n          \"maxLength\": 10\n        },\n        {\n          \"description\": \"The version of the signing profile.\"\n        }\n      ]\n    },\n    \"action\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The AWS Signer action permitted as part of cross-account permissions.\"\n        }\n      ]\n    },\n    \"principal\": {\n      \"\
  allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The AWS principal receiving cross-account permissions. This may be an IAM role or another AWS account ID.\"\n        }\n      ]\n    },\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"A unique identifier for the current profile revision.\"\n        }\n      ]\n    },\n    \"statementId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"A unique identifier for the cross-account permission statement.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"action\",\n    \"principal\",\n    \"statementId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-add-profile-permission-request-schema.json
tags:
- Code Signing
- IoT
- Lambda
- Security
title: AddProfilePermissionRequest
---
