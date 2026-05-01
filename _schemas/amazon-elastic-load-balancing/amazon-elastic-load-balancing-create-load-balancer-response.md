---
description: Response from the CreateLoadBalancer action
layout: schema
name: CreateLoadBalancerResponse
properties_list:
- description: Information about the load balancer
  name: loadBalancers
  type: array
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
schema_file: json-schema/amazon-elastic-load-balancing-create-load-balancer-response-schema.json
slug: amazon-elastic-load-balancing-create-load-balancer-response
source_filename: amazon-elastic-load-balancing-create-load-balancer-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-create-load-balancer-response-schema.json\",\n  \"title\": \"CreateLoadBalancerResponse\",\n  \"description\": \"Response from the CreateLoadBalancer action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"loadBalancers\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the load balancer\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LoadBalancer\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-create-load-balancer-response-schema.json
tags:
- Amazon Web Services
- High Availability
- Load Balancing
- Networking
- Scalability
title: CreateLoadBalancerResponse
---
