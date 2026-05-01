---
description: SignPayloadRequest schema from AWS Signer API
layout: schema
name: SignPayloadRequest
properties_list:
- description: ''
  name: profileName
  type: object
- description: ''
  name: profileOwner
  type: object
- description: ''
  name: payload
  type: object
- description: ''
  name: payloadFormat
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-sign-payload-request-schema.json
slug: amazon-signer-sign-payload-request
source_filename: amazon-signer-sign-payload-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-sign-payload-request-schema.json\",\n  \"title\": \"SignPayloadRequest\",\n  \"description\": \"SignPayloadRequest schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profileName\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-zA-Z0-9_]{2,}\",\n          \"minLength\": 2,\n          \"maxLength\": 64\n        },\n        {\n          \"description\": \"The name of the signing profile.\"\n        }\n      ]\n    },\n    \"profileOwner\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9]{12}$\",\n          \"minLength\": 12,\n          \"maxLength\": 12\n        },\n        {\n          \"description\": \"The AWS account ID of the profile owner.\"\n        }\n   \
  \   ]\n    },\n    \"payload\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 4096\n        },\n        {\n          \"description\": \"Specifies the object digest (hash) to sign.\"\n        }\n      ]\n    },\n    \"payloadFormat\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"Payload content type\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"profileName\",\n    \"payload\",\n    \"payloadFormat\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-sign-payload-request-schema.json
tags:
- Code Signing
- IoT
- Lambda
- Security
title: SignPayloadRequest
---
