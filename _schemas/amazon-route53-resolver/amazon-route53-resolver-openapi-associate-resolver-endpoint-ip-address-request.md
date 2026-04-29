---
description: AssociateResolverEndpointIpAddressRequest schema from openapi
layout: schema
name: AssociateResolverEndpointIpAddressRequest
properties_list:
- description: ''
  name: ResolverEndpointId
  type: object
- description: ''
  name: IpAddress
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-associate-resolver-endpoint-ip-address-request-schema.json
slug: amazon-route53-resolver-openapi-associate-resolver-endpoint-ip-address-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-associate-resolver-endpoint-ip-address-request-schema.json\",\n  \"title\": \"AssociateResolverEndpointIpAddressRequest\",\n  \"description\": \"AssociateResolverEndpointIpAddressRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverEndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Resolver endpoint that you want to associate IP addresses with.\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressUpdate\"\n        },\n        {\n          \"description\": \"Either the IPv4 address that you want to add to a Resolver endpoint or\
  \ a subnet ID. If you specify a subnet ID, Resolver chooses an IP address for you from the available IPs in the specified subnet.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResolverEndpointId\",\n    \"IpAddress\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-associate-resolver-endpoint-ip-address-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: AssociateResolverEndpointIpAddressRequest
---
