---
description: DescribeCustomRoutingAcceleratorRequest schema from Amazon Global Accelerator API
layout: schema
name: DescribeCustomRoutingAcceleratorRequest
properties_list:
- description: ''
  name: AcceleratorArn
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-describe-custom-routing-accelerator-request-schema.json
slug: global-accelerator-describe-custom-routing-accelerator-request
source_filename: global-accelerator-describe-custom-routing-accelerator-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-describe-custom-routing-accelerator-request-schema.json\",\n  \"title\": \"DescribeCustomRoutingAcceleratorRequest\",\n  \"description\": \"DescribeCustomRoutingAcceleratorRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AcceleratorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the accelerator to describe.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AcceleratorArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-describe-custom-routing-accelerator-request-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: DescribeCustomRoutingAcceleratorRequest
---
