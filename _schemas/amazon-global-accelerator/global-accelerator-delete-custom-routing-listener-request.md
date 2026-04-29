---
description: DeleteCustomRoutingListenerRequest schema from Amazon Global Accelerator API
layout: schema
name: DeleteCustomRoutingListenerRequest
properties_list:
- description: ''
  name: ListenerArn
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-delete-custom-routing-listener-request-schema.json
slug: global-accelerator-delete-custom-routing-listener-request
source_filename: global-accelerator-delete-custom-routing-listener-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-delete-custom-routing-listener-request-schema.json\",\n  \"title\": \"DeleteCustomRoutingListenerRequest\",\n  \"description\": \"DeleteCustomRoutingListenerRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ListenerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the listener to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ListenerArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-delete-custom-routing-listener-request-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: DeleteCustomRoutingListenerRequest
---
