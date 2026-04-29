---
description: DisassociateResolverEndpointIpAddressRequest schema from openapi
layout: schema
name: DisassociateResolverEndpointIpAddressRequest
properties_list:
- description: ''
  name: ResolverEndpointId
  type: object
- description: ''
  name: IpAddress
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-disassociate-resolver-endpoint-ip-address-request-schema.json
slug: amazon-route53-resolver-openapi-disassociate-resolver-endpoint-ip-address-request
source_filename: amazon-route53-resolver-openapi-disassociate-resolver-endpoint-ip-address-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-disassociate-resolver-endpoint-ip-address-request-schema.json\",\n  \"title\": \"DisassociateResolverEndpointIpAddressRequest\",\n  \"description\": \"DisassociateResolverEndpointIpAddressRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverEndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Resolver endpoint that you want to disassociate an IP address from.\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressUpdate\"\n        },\n        {\n          \"description\": \"The IPv4 address that you want to remove from a Resolver\
  \ endpoint.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResolverEndpointId\",\n    \"IpAddress\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-disassociate-resolver-endpoint-ip-address-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: DisassociateResolverEndpointIpAddressRequest
---
