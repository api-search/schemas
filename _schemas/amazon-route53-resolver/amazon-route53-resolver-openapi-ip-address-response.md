---
description: In the response to a <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_GetResolverEndpoint.html">GetResolverEndpoint</a> request, information about the IP addresses that the Resolver endpoint uses for DNS queries.
layout: schema
name: IpAddressResponse
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
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: ModificationTime
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-ip-address-response-schema.json
slug: amazon-route53-resolver-openapi-ip-address-response
source_filename: amazon-route53-resolver-openapi-ip-address-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-ip-address-response-schema.json\",\n  \"title\": \"IpAddressResponse\",\n  \"description\": \"In the response to a <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_GetResolverEndpoint.html\\\">GetResolverEndpoint</a> request, information about the IP addresses that the Resolver endpoint uses for DNS queries.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IpId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of one IP address.\"\n        }\n      ]\n    },\n    \"SubnetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetId\"\n        },\n        {\n          \"description\": \"\
  The ID of one subnet.\"\n        }\n      ]\n    },\n    \"Ip\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ip\"\n        },\n        {\n          \"description\": \"One IPv4 address that the Resolver endpoint uses for DNS queries.\"\n        }\n      ]\n    },\n    \"Ipv6\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ipv6\"\n        },\n        {\n          \"description\": \" One IPv6 address that the Resolver endpoint uses for DNS queries. \"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressStatus\"\n        },\n        {\n          \"description\": \"A status code that gives the current status of the request.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusMessage\"\n        },\n        {\n          \"description\": \"A message that provides additional\
  \ information about the status of the request.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rfc3339TimeString\"\n        },\n        {\n          \"description\": \"The date and time that the IP address was created, in Unix time format and Coordinated Universal Time (UTC).\"\n        }\n      ]\n    },\n    \"ModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rfc3339TimeString\"\n        },\n        {\n          \"description\": \"The date and time that the IP address was last modified, in Unix time format and Coordinated Universal Time (UTC).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-ip-address-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: IpAddressResponse
---
