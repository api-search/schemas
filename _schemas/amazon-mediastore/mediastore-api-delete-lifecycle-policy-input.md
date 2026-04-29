---
description: DeleteLifecyclePolicyInput schema from Amazon MediaStore API
layout: schema
name: DeleteLifecyclePolicyInput
properties_list:
- description: ''
  name: ContainerName
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-delete-lifecycle-policy-input-schema.json
slug: mediastore-api-delete-lifecycle-policy-input
source_filename: mediastore-api-delete-lifecycle-policy-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-delete-lifecycle-policy-input-schema.json\",\n  \"title\": \"DeleteLifecyclePolicyInput\",\n  \"description\": \"DeleteLifecyclePolicyInput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContainerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerName\"\n        },\n        {\n          \"description\": \"The name of the container that holds the object lifecycle policy.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ContainerName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-delete-lifecycle-policy-input-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DeleteLifecyclePolicyInput
---
