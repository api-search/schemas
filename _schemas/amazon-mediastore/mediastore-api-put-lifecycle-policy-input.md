---
description: PutLifecyclePolicyInput schema from Amazon MediaStore API
layout: schema
name: PutLifecyclePolicyInput
properties_list:
- description: ''
  name: ContainerName
  type: object
- description: ''
  name: LifecyclePolicy
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-put-lifecycle-policy-input-schema.json
slug: mediastore-api-put-lifecycle-policy-input
source_filename: mediastore-api-put-lifecycle-policy-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-put-lifecycle-policy-input-schema.json\",\n  \"title\": \"PutLifecyclePolicyInput\",\n  \"description\": \"PutLifecyclePolicyInput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContainerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerName\"\n        },\n        {\n          \"description\": \"The name of the container that you want to assign the object lifecycle policy to.\"\n        }\n      ]\n    },\n    \"LifecyclePolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecyclePolicy\"\n        },\n        {\n          \"description\": \"The object lifecycle policy to apply to the container.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ContainerName\"\
  ,\n    \"LifecyclePolicy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-put-lifecycle-policy-input-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: PutLifecyclePolicyInput
---
