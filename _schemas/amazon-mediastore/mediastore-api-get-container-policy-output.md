---
description: GetContainerPolicyOutput schema from Amazon MediaStore API
layout: schema
name: GetContainerPolicyOutput
properties_list:
- description: ''
  name: Policy
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-get-container-policy-output-schema.json
slug: mediastore-api-get-container-policy-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-get-container-policy-output-schema.json\",\n  \"title\": \"GetContainerPolicyOutput\",\n  \"description\": \"GetContainerPolicyOutput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerPolicy\"\n        },\n        {\n          \"description\": \"The contents of the access policy.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Policy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-get-container-policy-output-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: GetContainerPolicyOutput
---
