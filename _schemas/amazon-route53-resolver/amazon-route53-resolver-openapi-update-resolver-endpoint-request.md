---
description: UpdateResolverEndpointRequest schema from openapi
layout: schema
name: UpdateResolverEndpointRequest
properties_list:
- description: ''
  name: ResolverEndpointId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: ResolverEndpointType
  type: object
- description: ''
  name: UpdateIpAddresses
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-update-resolver-endpoint-request-schema.json
slug: amazon-route53-resolver-openapi-update-resolver-endpoint-request
source_filename: amazon-route53-resolver-openapi-update-resolver-endpoint-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-resolver-endpoint-request-schema.json\",\n  \"title\": \"UpdateResolverEndpointRequest\",\n  \"description\": \"UpdateResolverEndpointRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverEndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Resolver endpoint that you want to update.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the Resolver endpoint that you want to update.\"\n        }\n      ]\n    },\n    \"ResolverEndpointType\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/ResolverEndpointType\"\n        },\n        {\n          \"description\": \" Specifies the endpoint type for what type of IP address the endpoint uses to forward DNS queries. \"\n        }\n      ]\n    },\n    \"UpdateIpAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateIpAddresses\"\n        },\n        {\n          \"description\": \" Updates the Resolver endpoint type to IpV4, Ipv6, or dual-stack. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResolverEndpointId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-resolver-endpoint-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: UpdateResolverEndpointRequest
---
