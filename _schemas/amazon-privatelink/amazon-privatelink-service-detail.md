---
description: ServiceDetail schema from Amazon PrivateLink API
layout: schema
name: ServiceDetail
properties_list:
- description: Name of the endpoint service
  name: ServiceName
  type: string
- description: Unique ID of the endpoint service
  name: ServiceId
  type: string
- description: Type of service
  name: ServiceType
  type: array
- description: Availability zones
  name: AvailabilityZones
  type: array
- description: Owner AWS account ID
  name: Owner
  type: string
- description: Base DNS names for the endpoint service
  name: BaseEndpointDnsNames
  type: array
- description: Private DNS name
  name: PrivateDnsName
  type: string
- description: Whether acceptance is required
  name: AcceptanceRequired
  type: boolean
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-service-detail-schema.json
slug: amazon-privatelink-service-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-service-detail-schema.json\",\n  \"title\": \"ServiceDetail\",\n  \"description\": \"ServiceDetail schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the endpoint service\"\n    },\n    \"ServiceId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID of the endpoint service\"\n    },\n    \"ServiceType\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Type of service\"\n    },\n    \"AvailabilityZones\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Availability zones\"\n    },\n    \"Owner\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Owner AWS account ID\"\n    },\n    \"BaseEndpointDnsNames\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Base DNS names for the endpoint service\"\n    },\n    \"PrivateDnsName\": {\n      \"type\": \"string\",\n      \"description\": \"Private DNS name\"\n    },\n    \"AcceptanceRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether acceptance is required\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-service-detail-schema.json
tags:
- AWS
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: ServiceDetail
---
