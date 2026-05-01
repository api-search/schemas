---
description: A complex type for a listener for a custom routing accelerator.
layout: schema
name: CustomRoutingListener
properties_list:
- description: ''
  name: ListenerArn
  type: object
- description: ''
  name: PortRanges
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-custom-routing-listener-schema.json
slug: global-accelerator-custom-routing-listener
source_filename: global-accelerator-custom-routing-listener-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-custom-routing-listener-schema.json\",\n  \"title\": \"CustomRoutingListener\",\n  \"description\": \"A complex type for a listener for a custom routing accelerator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ListenerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the listener.\"\n        }\n      ]\n    },\n    \"PortRanges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortRanges\"\n        },\n        {\n          \"description\": \"<p>The port range to support for connections from clients to your accelerator.</p> <p>Separately, you set port ranges for endpoints. For more information, see\
  \ <a href=\\\"https://docs.aws.amazon.com/global-accelerator/latest/dg/about-custom-routing-endpoints.html\\\">About endpoints for custom routing accelerators</a>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-custom-routing-listener-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: CustomRoutingListener
---
