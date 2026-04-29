---
description: The ACM certificate that is used to sign your code.
layout: schema
name: SigningMaterial
properties_list:
- description: ''
  name: certificateArn
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-signing-material-schema.json
slug: amazon-signer-signing-material
source_filename: amazon-signer-signing-material-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-material-schema.json\",\n  \"title\": \"SigningMaterial\",\n  \"description\": \"The ACM certificate that is used to sign your code.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateArn\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the certificates that is used to sign your code.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"certificateArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-material-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: SigningMaterial
---
