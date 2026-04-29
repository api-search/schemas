---
description: A complex type for a range of ports for a listener.
layout: schema
name: PortRange
properties_list:
- description: ''
  name: FromPort
  type: object
- description: ''
  name: ToPort
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-port-range-schema.json
slug: global-accelerator-port-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-port-range-schema.json\",\n  \"title\": \"PortRange\",\n  \"description\": \"A complex type for a range of ports for a listener.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FromPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\n        },\n        {\n          \"description\": \"The first port in the range of ports, inclusive.\"\n        }\n      ]\n    },\n    \"ToPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\n        },\n        {\n          \"description\": \"The last port in the range of ports, inclusive.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-port-range-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: PortRange
---
