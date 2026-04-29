---
description: DeleteVpcEndpointServiceConfigurationsRequest schema from Amazon PrivateLink API
layout: schema
name: DeleteVpcEndpointServiceConfigurationsRequest
properties_list:
- description: IDs of endpoint services to delete
  name: ServiceId
  type: array
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-delete-vpc-endpoint-service-configurations-request-schema.json
slug: amazon-privatelink-delete-vpc-endpoint-service-configurations-request
source_filename: amazon-privatelink-delete-vpc-endpoint-service-configurations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-delete-vpc-endpoint-service-configurations-request-schema.json\",\n  \"title\": \"DeleteVpcEndpointServiceConfigurationsRequest\",\n  \"description\": \"DeleteVpcEndpointServiceConfigurationsRequest schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceId\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IDs of endpoint services to delete\"\n    }\n  },\n  \"required\": [\n    \"ServiceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-delete-vpc-endpoint-service-configurations-request-schema.json
tags:
- AWS
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: DeleteVpcEndpointServiceConfigurationsRequest
---
