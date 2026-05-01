---
description: CreateCustomRoutingListenerResponse schema from Amazon Global Accelerator API
layout: schema
name: CreateCustomRoutingListenerResponse
properties_list:
- description: ''
  name: Listener
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-create-custom-routing-listener-response-schema.json
slug: global-accelerator-create-custom-routing-listener-response
source_filename: global-accelerator-create-custom-routing-listener-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-create-custom-routing-listener-response-schema.json\",\n  \"title\": \"CreateCustomRoutingListenerResponse\",\n  \"description\": \"CreateCustomRoutingListenerResponse schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Listener\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomRoutingListener\"\n        },\n        {\n          \"description\": \"The listener that you've created for a custom routing accelerator.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-create-custom-routing-listener-response-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: CreateCustomRoutingListenerResponse
---
