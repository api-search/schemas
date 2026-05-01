---
description: Describes a load balancer
layout: schema
name: LoadBalancer
properties_list:
- description: The Amazon Resource Name (ARN) of the load balancer
  name: loadBalancerArn
  type: string
- description: The public DNS name of the load balancer
  name: dnsName
  type: string
- description: The ID of the Amazon Route 53 hosted zone for the load balancer
  name: canonicalHostedZoneId
  type: string
- description: The date and time the load balancer was created
  name: createdTime
  type: string
- description: The name of the load balancer
  name: loadBalancerName
  type: string
- description: The scheme of the load balancer
  name: scheme
  type: string
- description: The ID of the VPC for the load balancer
  name: vpcId
  type: string
- description: The state of the load balancer
  name: state
  type: object
- description: The type of load balancer
  name: type
  type: string
- description: The subnets for the load balancer
  name: availabilityZones
  type: array
- description: The IDs of the security groups for the load balancer
  name: securityGroups
  type: array
- description: The type of IP addresses used by the subnets
  name: ipAddressType
  type: string
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
schema_file: json-schema/amazon-elastic-load-balancing-load-balancer-schema.json
slug: amazon-elastic-load-balancing-load-balancer
source_filename: amazon-elastic-load-balancing-load-balancer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-load-balancer-schema.json\",\n  \"title\": \"LoadBalancer\",\n  \"description\": \"Describes a load balancer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"loadBalancerArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the load balancer\"\n    },\n    \"dnsName\": {\n      \"type\": \"string\",\n      \"description\": \"The public DNS name of the load balancer\"\n    },\n    \"canonicalHostedZoneId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Amazon Route 53 hosted zone for the load balancer\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the load balancer was created\"\n    },\n    \"\
  loadBalancerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the load balancer\"\n    },\n    \"scheme\": {\n      \"type\": \"string\",\n      \"description\": \"The scheme of the load balancer\",\n      \"enum\": [\n        \"internet-facing\",\n        \"internal\"\n      ]\n    },\n    \"vpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the VPC for the load balancer\"\n    },\n    \"state\": {\n      \"type\": \"object\",\n      \"description\": \"The state of the load balancer\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"The state code\",\n          \"enum\": [\n            \"active\",\n            \"provisioning\",\n            \"active_impaired\",\n            \"failed\"\n          ]\n        },\n        \"reason\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the state\"\n        }\n      }\n    },\n    \"type\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"The type of load balancer\",\n      \"enum\": [\n        \"application\",\n        \"network\",\n        \"gateway\"\n      ]\n    },\n    \"availabilityZones\": {\n      \"type\": \"array\",\n      \"description\": \"The subnets for the load balancer\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"zoneName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the Availability Zone\"\n          },\n          \"subnetId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the subnet\"\n          }\n        }\n      }\n    },\n    \"securityGroups\": {\n      \"type\": \"array\",\n      \"description\": \"The IDs of the security groups for the load balancer\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"ipAddressType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of IP addresses used\
  \ by the subnets\",\n      \"enum\": [\n        \"ipv4\",\n        \"dualstack\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-load-balancer-schema.json
tags:
- Amazon Web Services
- High Availability
- Load Balancing
- Networking
- Scalability
title: LoadBalancer
---
