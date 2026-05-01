---
description: In an <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_UpdateResolverEndpoint.html">UpdateResolverEndpoint</a> request, information about an IP address to update.
layout: schema
name: IpAddressUpdate
properties_list:
- description: ''
  name: IpId
  type: object
- description: ''
  name: SubnetId
  type: object
- description: ''
  name: Ip
  type: object
- description: ''
  name: Ipv6
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-ip-address-update-schema.json
slug: amazon-route53-resolver-openapi-ip-address-update
source_filename: amazon-route53-resolver-openapi-ip-address-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-ip-address-update-schema.json\",\n  \"title\": \"IpAddressUpdate\",\n  \"description\": \"In an <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_UpdateResolverEndpoint.html\\\">UpdateResolverEndpoint</a> request, information about an IP address to update.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IpId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \" <i>Only when removing an IP address from a Resolver endpoint</i>: The ID of the IP address that you want to remove. To get this ID, use <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_GetResolverEndpoint.html\\\">GetResolverEndpoint</a>.\"\
  \n        }\n      ]\n    },\n    \"SubnetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetId\"\n        },\n        {\n          \"description\": \"The ID of the subnet that includes the IP address that you want to update. To get this ID, use <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_GetResolverEndpoint.html\\\">GetResolverEndpoint</a>.\"\n        }\n      ]\n    },\n    \"Ip\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ip\"\n        },\n        {\n          \"description\": \"The new IPv4 address.\"\n        }\n      ]\n    },\n    \"Ipv6\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ipv6\"\n        },\n        {\n          \"description\": \" The new IPv6 address. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-ip-address-update-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: IpAddressUpdate
---
