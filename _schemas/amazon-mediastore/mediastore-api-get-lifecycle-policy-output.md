---
description: GetLifecyclePolicyOutput schema from Amazon MediaStore API
layout: schema
name: GetLifecyclePolicyOutput
properties_list:
- description: ''
  name: LifecyclePolicy
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-get-lifecycle-policy-output-schema.json
slug: mediastore-api-get-lifecycle-policy-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-get-lifecycle-policy-output-schema.json\",\n  \"title\": \"GetLifecyclePolicyOutput\",\n  \"description\": \"GetLifecyclePolicyOutput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LifecyclePolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecyclePolicy\"\n        },\n        {\n          \"description\": \"The object lifecycle policy that is assigned to the container.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LifecyclePolicy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-get-lifecycle-policy-output-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: GetLifecyclePolicyOutput
---
