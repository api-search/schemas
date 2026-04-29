---
description: The image format of a code signing platform or profile.
layout: schema
name: SigningImageFormat
properties_list:
- description: ''
  name: supportedFormats
  type: object
- description: ''
  name: defaultFormat
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-signing-image-format-schema.json
slug: amazon-signer-signing-image-format
source_filename: amazon-signer-signing-image-format-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-image-format-schema.json\",\n  \"title\": \"SigningImageFormat\",\n  \"description\": \"The image format of a code signing platform or profile.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"supportedFormats\": {\n      \"allOf\": [\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/ImageFormat\"\n          }\n        },\n        {\n          \"description\": \"The supported formats of a code signing image.\"\n        }\n      ]\n    },\n    \"defaultFormat\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"enum\": [\n            \"JSON\",\n            \"JSONEmbedded\",\n            \"JSONDetached\"\n          ]\n        },\n        {\n          \"description\": \"The default format\
  \ of a code signing image.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"supportedFormats\",\n    \"defaultFormat\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-image-format-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: SigningImageFormat
---
