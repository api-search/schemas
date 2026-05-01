---
description: Describes the state of a Classic Load Balancer.
layout: schema
name: LoadBalancerState
properties_list:
- description: ''
  name: LoadBalancerName
  type: object
- description: ''
  name: State
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-load-balancer-state-schema.json
slug: ec2-auto-scaling-load-balancer-state
source_filename: ec2-auto-scaling-load-balancer-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-load-balancer-state-schema.json\",\n  \"title\": \"LoadBalancerState\",\n  \"description\": \"Describes the state of a Classic Load Balancer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LoadBalancerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the load balancer.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>One of the following load balancer states:</p> <ul> <li> <p> <code>Adding</code> - The Auto Scaling instances are being registered with the load balancer.</p> </li> <li> <p> <code>Added</code>\
  \ - All Auto Scaling instances are registered with the load balancer.</p> </li> <li> <p> <code>InService</code> - At least one Auto Scaling instance passed an <code>ELB</code> health check.</p> </li> <li> <p> <code>Removing</code> - The Auto Scaling instances are being deregistered from the load balancer. If connection draining is enabled, Elastic Load Balancing waits for in-flight requests to complete before deregistering the instances.</p> </li> <li> <p> <code>Removed</code> - All Auto Scaling instances are deregistered from the load balancer.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-load-balancer-state-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: LoadBalancerState
---
