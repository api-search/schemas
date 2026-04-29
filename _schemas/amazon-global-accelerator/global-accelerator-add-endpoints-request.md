---
description: AddEndpointsRequest schema from Amazon Global Accelerator API
layout: schema
name: AddEndpointsRequest
properties_list:
- description: ''
  name: EndpointConfigurations
  type: object
- description: ''
  name: EndpointGroupArn
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-add-endpoints-request-schema.json
slug: global-accelerator-add-endpoints-request
source_filename: global-accelerator-add-endpoints-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-add-endpoints-request-schema.json\",\n  \"title\": \"AddEndpointsRequest\",\n  \"description\": \"AddEndpointsRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointConfigurations\"\n        },\n        {\n          \"description\": \"The list of endpoint objects.\"\n        }\n      ]\n    },\n    \"EndpointGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the endpoint group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointConfigurations\",\n    \"EndpointGroupArn\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-add-endpoints-request-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: AddEndpointsRequest
---
