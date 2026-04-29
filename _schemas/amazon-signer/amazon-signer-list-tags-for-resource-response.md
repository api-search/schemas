---
description: ListTagsForResourceResponse schema from AWS Signer API
layout: schema
name: ListTagsForResourceResponse
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-list-tags-for-resource-response-schema.json
slug: amazon-signer-list-tags-for-resource-response
source_filename: amazon-signer-list-tags-for-resource-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-list-tags-for-resource-response-schema.json\",\n  \"title\": \"ListTagsForResourceResponse\",\n  \"description\": \"ListTagsForResourceResponse schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"minProperties\": 1,\n          \"maxProperties\": 200,\n          \"additionalProperties\": {\n            \"$ref\": \"#/components/schemas/TagValue\"\n          }\n        },\n        {\n          \"description\": \"A list of tags associated with the signing profile.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-list-tags-for-resource-response-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: ListTagsForResourceResponse
---
