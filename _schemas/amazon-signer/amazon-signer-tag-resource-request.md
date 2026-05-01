---
description: TagResourceRequest schema from AWS Signer API
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-tag-resource-request-schema.json
slug: amazon-signer-tag-resource-request
source_filename: amazon-signer-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"minProperties\": 1,\n          \"maxProperties\": 200,\n          \"additionalProperties\": {\n            \"$ref\": \"#/components/schemas/TagValue\"\n          }\n        },\n        {\n          \"description\": \"One or more tags to be associated with the signing profile.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-tag-resource-request-schema.json
tags:
- Code Signing
- IoT
- Lambda
- Security
title: TagResourceRequest
---
