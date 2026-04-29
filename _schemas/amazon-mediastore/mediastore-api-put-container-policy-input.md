---
description: PutContainerPolicyInput schema from Amazon MediaStore API
layout: schema
name: PutContainerPolicyInput
properties_list:
- description: ''
  name: ContainerName
  type: object
- description: ''
  name: Policy
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-put-container-policy-input-schema.json
slug: mediastore-api-put-container-policy-input
source_filename: mediastore-api-put-container-policy-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-put-container-policy-input-schema.json\",\n  \"title\": \"PutContainerPolicyInput\",\n  \"description\": \"PutContainerPolicyInput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContainerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerName\"\n        },\n        {\n          \"description\": \"The name of the container.\"\n        }\n      ]\n    },\n    \"Policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerPolicy\"\n        },\n        {\n          \"description\": \"<p>The contents of the policy, which includes the following: </p> <ul> <li> <p>One <code>Version</code> tag</p> </li> <li> <p>One <code>Statement</code> tag that contains the standard tags for\
  \ the policy.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ContainerName\",\n    \"Policy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-put-container-policy-input-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PutContainerPolicyInput
---
