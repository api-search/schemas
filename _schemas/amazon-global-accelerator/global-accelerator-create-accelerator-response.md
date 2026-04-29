---
description: CreateAcceleratorResponse schema from Amazon Global Accelerator API
layout: schema
name: CreateAcceleratorResponse
properties_list:
- description: ''
  name: Accelerator
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-create-accelerator-response-schema.json
slug: global-accelerator-create-accelerator-response
source_filename: global-accelerator-create-accelerator-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-create-accelerator-response-schema.json\",\n  \"title\": \"CreateAcceleratorResponse\",\n  \"description\": \"CreateAcceleratorResponse schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Accelerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Accelerator\"\n        },\n        {\n          \"description\": \"The accelerator that is created by specifying a listener and the supported IP address types.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-create-accelerator-response-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: CreateAcceleratorResponse
---
