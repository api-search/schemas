---
description: CreateCustomRoutingListenerRequest schema from Amazon Global Accelerator API
layout: schema
name: CreateCustomRoutingListenerRequest
properties_list:
- description: ''
  name: AcceleratorArn
  type: object
- description: ''
  name: PortRanges
  type: object
- description: ''
  name: IdempotencyToken
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-create-custom-routing-listener-request-schema.json
slug: global-accelerator-create-custom-routing-listener-request
source_filename: global-accelerator-create-custom-routing-listener-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-create-custom-routing-listener-request-schema.json\",\n  \"title\": \"CreateCustomRoutingListenerRequest\",\n  \"description\": \"CreateCustomRoutingListenerRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AcceleratorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the accelerator for a custom routing listener.\"\n        }\n      ]\n    },\n    \"PortRanges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortRanges\"\n        },\n        {\n          \"description\": \"<p>The port range to support for connections from clients to your accelerator.</p>\
  \ <p>Separately, you set port ranges for endpoints. For more information, see <a href=\\\"https://docs.aws.amazon.com/global-accelerator/latest/dg/about-custom-routing-endpoints.html\\\">About endpoints for custom routing accelerators</a>.</p>\"\n        }\n      ]\n    },\n    \"IdempotencyToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyToken\"\n        },\n        {\n          \"description\": \"A unique, case-sensitive identifier that you provide to ensure the idempotency\\u2014that is, the uniqueness\\u2014of the request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AcceleratorArn\",\n    \"PortRanges\",\n    \"IdempotencyToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-create-custom-routing-listener-request-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: CreateCustomRoutingListenerRequest
---
