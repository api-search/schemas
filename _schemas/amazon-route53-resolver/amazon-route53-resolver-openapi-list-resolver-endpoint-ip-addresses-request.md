---
description: ListResolverEndpointIpAddressesRequest schema from openapi
layout: schema
name: ListResolverEndpointIpAddressesRequest
properties_list:
- description: ''
  name: ResolverEndpointId
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-resolver-endpoint-ip-addresses-request-schema.json
slug: amazon-route53-resolver-openapi-list-resolver-endpoint-ip-addresses-request
source_filename: amazon-route53-resolver-openapi-list-resolver-endpoint-ip-addresses-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-endpoint-ip-addresses-request-schema.json\",\n  \"title\": \"ListResolverEndpointIpAddressesRequest\",\n  \"description\": \"ListResolverEndpointIpAddressesRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverEndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Resolver endpoint that you want to get IP addresses for.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of IP addresses that you want to return in the response to a <code>ListResolverEndpointIpAddresses</code>\
  \ request. If you don't specify a value for <code>MaxResults</code>, Resolver returns up to 100 IP addresses. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>For the first <code>ListResolverEndpointIpAddresses</code> request, omit this value.</p> <p>If the specified Resolver endpoint has more than <code>MaxResults</code> IP addresses, you can submit another <code>ListResolverEndpointIpAddresses</code> request to get the next group of IP addresses. In the next request, specify the value of <code>NextToken</code> from the previous response. </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResolverEndpointId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-endpoint-ip-addresses-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ListResolverEndpointIpAddressesRequest
---
