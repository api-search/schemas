---
description: Provides information about the IP address type in response to <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_UpdateResolverEndpoint.html">UpdateResolverEndpoint</a>.
layout: schema
name: UpdateIpAddress
properties_list:
- description: ''
  name: IpId
  type: object
- description: ''
  name: Ipv6
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-update-ip-address-schema.json
slug: amazon-route53-resolver-openapi-update-ip-address
source_filename: amazon-route53-resolver-openapi-update-ip-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-ip-address-schema.json\",\n  \"title\": \"UpdateIpAddress\",\n  \"description\": \" Provides information about the IP address type in response to <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_UpdateResolverEndpoint.html\\\">UpdateResolverEndpoint</a>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IpId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \" The ID of the IP address, specified by the <code>ResolverEndpointId</code>. \"\n        }\n      ]\n    },\n    \"Ipv6\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ipv6\"\n        },\n        {\n          \"description\": \" The\
  \ IPv6 address that you want to use for DNS queries. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IpId\",\n    \"Ipv6\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-ip-address-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: UpdateIpAddress
---
