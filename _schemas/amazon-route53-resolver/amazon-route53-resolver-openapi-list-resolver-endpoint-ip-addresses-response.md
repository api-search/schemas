---
description: ListResolverEndpointIpAddressesResponse schema from openapi
layout: schema
name: ListResolverEndpointIpAddressesResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: IpAddresses
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-resolver-endpoint-ip-addresses-response-schema.json
slug: amazon-route53-resolver-openapi-list-resolver-endpoint-ip-addresses-response
source_filename: amazon-route53-resolver-openapi-list-resolver-endpoint-ip-addresses-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-endpoint-ip-addresses-response-schema.json\",\n  \"title\": \"ListResolverEndpointIpAddressesResponse\",\n  \"description\": \"ListResolverEndpointIpAddressesResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If the specified endpoint has more than <code>MaxResults</code> IP addresses, you can submit another <code>ListResolverEndpointIpAddresses</code> request to get the next group of IP addresses. In the next request, specify the value of <code>NextToken</code> from the previous response. \"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The value that you specified for <code>MaxResults</code> in the request.\"\n        }\n      ]\n    },\n    \"IpAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressesResponse\"\n        },\n        {\n          \"description\": \"Information about the IP addresses in your VPC that DNS queries originate from (for outbound endpoints) or that you forward DNS queries to (for inbound endpoints).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-endpoint-ip-addresses-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ListResolverEndpointIpAddressesResponse
---
