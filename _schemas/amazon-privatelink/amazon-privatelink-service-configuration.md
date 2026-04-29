---
description: ServiceConfiguration schema from Amazon PrivateLink API
layout: schema
name: ServiceConfiguration
properties_list:
- description: Type of service (Interface or Gateway)
  name: ServiceType
  type: array
- description: Unique ID of the endpoint service
  name: ServiceId
  type: string
- description: Name of the endpoint service
  name: ServiceName
  type: string
- description: State of the endpoint service
  name: ServiceState
  type: string
- description: Whether connections require acceptance
  name: AcceptanceRequired
  type: boolean
- description: Availability zones where the service is available
  name: AvailabilityZones
  type: array
- description: ARNs of Network Load Balancers
  name: NetworkLoadBalancerArns
  type: array
- description: Private DNS name
  name: PrivateDnsName
  type: string
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-service-configuration-schema.json
slug: amazon-privatelink-service-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-service-configuration-schema.json\",\n  \"title\": \"ServiceConfiguration\",\n  \"description\": \"ServiceConfiguration schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceType\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Type of service (Interface or Gateway)\"\n    },\n    \"ServiceId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID of the endpoint service\"\n    },\n    \"ServiceName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the endpoint service\"\n    },\n    \"ServiceState\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Pending\",\n        \"Available\",\n        \"Deleting\",\n        \"Deleted\"\
  ,\n        \"Failed\"\n      ],\n      \"description\": \"State of the endpoint service\"\n    },\n    \"AcceptanceRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether connections require acceptance\"\n    },\n    \"AvailabilityZones\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Availability zones where the service is available\"\n    },\n    \"NetworkLoadBalancerArns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"ARNs of Network Load Balancers\"\n    },\n    \"PrivateDnsName\": {\n      \"type\": \"string\",\n      \"description\": \"Private DNS name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-service-configuration-schema.json
tags:
- AWS
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: ServiceConfiguration
---
