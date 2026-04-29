---
description: DeleteCustomRoutingEndpointGroupRequest schema from Amazon Global Accelerator API
layout: schema
name: DeleteCustomRoutingEndpointGroupRequest
properties_list:
- description: ''
  name: EndpointGroupArn
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-delete-custom-routing-endpoint-group-request-schema.json
slug: global-accelerator-delete-custom-routing-endpoint-group-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-delete-custom-routing-endpoint-group-request-schema.json\",\n  \"title\": \"DeleteCustomRoutingEndpointGroupRequest\",\n  \"description\": \"DeleteCustomRoutingEndpointGroupRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the endpoint group to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointGroupArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-delete-custom-routing-endpoint-group-request-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: DeleteCustomRoutingEndpointGroupRequest
---
