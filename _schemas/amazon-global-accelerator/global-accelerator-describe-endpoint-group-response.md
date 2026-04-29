---
description: DescribeEndpointGroupResponse schema from Amazon Global Accelerator API
layout: schema
name: DescribeEndpointGroupResponse
properties_list:
- description: ''
  name: EndpointGroup
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-describe-endpoint-group-response-schema.json
slug: global-accelerator-describe-endpoint-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-describe-endpoint-group-response-schema.json\",\n  \"title\": \"DescribeEndpointGroupResponse\",\n  \"description\": \"DescribeEndpointGroupResponse schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointGroup\"\n        },\n        {\n          \"description\": \"The description of an endpoint group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-describe-endpoint-group-response-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: DescribeEndpointGroupResponse
---
