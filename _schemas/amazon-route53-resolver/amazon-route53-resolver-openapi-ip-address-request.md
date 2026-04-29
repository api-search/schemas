---
description: In a <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_CreateResolverEndpoint.html">CreateResolverEndpoint</a> request, the IP address that DNS queries originate from (for outbound endpoints) or that you forward DNS queries to (for inbound endpoints). <code>IpAddressRequest</code> also includes the ID of the subnet that contains the IP address.
layout: schema
name: IpAddressRequest
properties_list:
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
schema_file: json-schema/amazon-route53-resolver-openapi-ip-address-request-schema.json
slug: amazon-route53-resolver-openapi-ip-address-request
source_filename: amazon-route53-resolver-openapi-ip-address-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-ip-address-request-schema.json\",\n  \"title\": \"IpAddressRequest\",\n  \"description\": \"In a <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_CreateResolverEndpoint.html\\\">CreateResolverEndpoint</a> request, the IP address that DNS queries originate from (for outbound endpoints) or that you forward DNS queries to (for inbound endpoints). <code>IpAddressRequest</code> also includes the ID of the subnet that contains the IP address.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SubnetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetId\"\n        },\n        {\n          \"description\": \"The ID of the subnet that contains the IP address. \"\n        }\n      ]\n    },\n\
  \    \"Ip\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ip\"\n        },\n        {\n          \"description\": \"The IPv4 address that you want to use for DNS queries.\"\n        }\n      ]\n    },\n    \"Ipv6\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ipv6\"\n        },\n        {\n          \"description\": \" The IPv6 address that you want to use for DNS queries. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SubnetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-ip-address-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: IpAddressRequest
---
