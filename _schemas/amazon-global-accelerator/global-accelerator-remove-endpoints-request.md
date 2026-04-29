---
description: RemoveEndpointsRequest schema from Amazon Global Accelerator API
layout: schema
name: RemoveEndpointsRequest
properties_list:
- description: ''
  name: EndpointIdentifiers
  type: object
- description: ''
  name: EndpointGroupArn
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-remove-endpoints-request-schema.json
slug: global-accelerator-remove-endpoints-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-remove-endpoints-request-schema.json\",\n  \"title\": \"RemoveEndpointsRequest\",\n  \"description\": \"RemoveEndpointsRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointIdentifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointIdentifiers\"\n        },\n        {\n          \"description\": \"The identifiers of the endpoints that you want to remove.\"\n        }\n      ]\n    },\n    \"EndpointGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the endpoint group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointIdentifiers\"\
  ,\n    \"EndpointGroupArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-remove-endpoints-request-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: RemoveEndpointsRequest
---
