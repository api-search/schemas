---
description: DescribeCustomRoutingListenerResponse schema from Amazon Global Accelerator API
layout: schema
name: DescribeCustomRoutingListenerResponse
properties_list:
- description: ''
  name: Listener
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-describe-custom-routing-listener-response-schema.json
slug: global-accelerator-describe-custom-routing-listener-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-describe-custom-routing-listener-response-schema.json\",\n  \"title\": \"DescribeCustomRoutingListenerResponse\",\n  \"description\": \"DescribeCustomRoutingListenerResponse schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Listener\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomRoutingListener\"\n        },\n        {\n          \"description\": \"The description of a listener for a custom routing accelerator.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-describe-custom-routing-listener-response-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: DescribeCustomRoutingListenerResponse
---
