---
description: In a <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_CreateResolverRule.html">CreateResolverRule</a> request, an array of the IPs that you want to forward DNS queries to.
layout: schema
name: TargetAddress
properties_list:
- description: ''
  name: Ip
  type: object
- description: ''
  name: Port
  type: object
- description: ''
  name: Ipv6
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-target-address-schema.json
slug: amazon-route53-resolver-openapi-target-address
source_filename: amazon-route53-resolver-openapi-target-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-target-address-schema.json\",\n  \"title\": \"TargetAddress\",\n  \"description\": \"In a <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_CreateResolverRule.html\\\">CreateResolverRule</a> request, an array of the IPs that you want to forward DNS queries to.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Ip\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ip\"\n        },\n        {\n          \"description\": \"One IPv4 address that you want to forward DNS queries to.\"\n        }\n      ]\n    },\n    \"Port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Port\"\n        },\n        {\n          \"description\": \"The port at <code>Ip</code> that you\
  \ want to forward DNS queries to.\"\n        }\n      ]\n    },\n    \"Ipv6\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ipv6\"\n        },\n        {\n          \"description\": \" One IPv6 address that you want to forward DNS queries to. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-target-address-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: TargetAddress
---
