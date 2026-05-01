---
description: UpdateCustomRoutingAcceleratorResponse schema from Amazon Global Accelerator API
layout: schema
name: UpdateCustomRoutingAcceleratorResponse
properties_list:
- description: ''
  name: Accelerator
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-update-custom-routing-accelerator-response-schema.json
slug: global-accelerator-update-custom-routing-accelerator-response
source_filename: global-accelerator-update-custom-routing-accelerator-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-custom-routing-accelerator-response-schema.json\",\n  \"title\": \"UpdateCustomRoutingAcceleratorResponse\",\n  \"description\": \"UpdateCustomRoutingAcceleratorResponse schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Accelerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomRoutingAccelerator\"\n        },\n        {\n          \"description\": \"Information about the updated custom routing accelerator.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-custom-routing-accelerator-response-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: UpdateCustomRoutingAcceleratorResponse
---
