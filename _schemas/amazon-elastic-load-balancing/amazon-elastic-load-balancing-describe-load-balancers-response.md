---
description: Response from the DescribeLoadBalancers action
layout: schema
name: DescribeLoadBalancersResponse
properties_list:
- description: Information about the load balancers
  name: loadBalancers
  type: array
- description: The marker to use for the next set of results
  name: nextMarker
  type: string
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
schema_file: json-schema/amazon-elastic-load-balancing-describe-load-balancers-response-schema.json
slug: amazon-elastic-load-balancing-describe-load-balancers-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-describe-load-balancers-response-schema.json\",\n  \"title\": \"DescribeLoadBalancersResponse\",\n  \"description\": \"Response from the DescribeLoadBalancers action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"loadBalancers\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the load balancers\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LoadBalancer\"\n      }\n    },\n    \"nextMarker\": {\n      \"type\": \"string\",\n      \"description\": \"The marker to use for the next set of results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-describe-load-balancers-response-schema.json
tags:
- Amazon Web Services
- AWS
- High Availability
- Load Balancing
- Networking
- Scalability
title: DescribeLoadBalancersResponse
---
