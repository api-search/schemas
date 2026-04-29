---
description: UpdateAcceleratorAttributesResponse schema from Amazon Global Accelerator API
layout: schema
name: UpdateAcceleratorAttributesResponse
properties_list:
- description: ''
  name: AcceleratorAttributes
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-update-accelerator-attributes-response-schema.json
slug: global-accelerator-update-accelerator-attributes-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-accelerator-attributes-response-schema.json\",\n  \"title\": \"UpdateAcceleratorAttributesResponse\",\n  \"description\": \"UpdateAcceleratorAttributesResponse schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AcceleratorAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AcceleratorAttributes\"\n        },\n        {\n          \"description\": \"Updated attributes for the accelerator.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-accelerator-attributes-response-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: UpdateAcceleratorAttributesResponse
---
