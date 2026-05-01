---
description: UpdateListenerResponse schema from Amazon Global Accelerator API
layout: schema
name: UpdateListenerResponse
properties_list:
- description: ''
  name: Listener
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-update-listener-response-schema.json
slug: global-accelerator-update-listener-response
source_filename: global-accelerator-update-listener-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-listener-response-schema.json\",\n  \"title\": \"UpdateListenerResponse\",\n  \"description\": \"UpdateListenerResponse schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Listener\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Listener\"\n        },\n        {\n          \"description\": \"Information for the updated listener.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-listener-response-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: UpdateListenerResponse
---
