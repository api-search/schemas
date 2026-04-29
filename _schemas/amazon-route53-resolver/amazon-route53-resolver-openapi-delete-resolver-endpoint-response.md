---
description: DeleteResolverEndpointResponse schema from openapi
layout: schema
name: DeleteResolverEndpointResponse
properties_list:
- description: ''
  name: ResolverEndpoint
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-delete-resolver-endpoint-response-schema.json
slug: amazon-route53-resolver-openapi-delete-resolver-endpoint-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-delete-resolver-endpoint-response-schema.json\",\n  \"title\": \"DeleteResolverEndpointResponse\",\n  \"description\": \"DeleteResolverEndpointResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverEndpoint\"\n        },\n        {\n          \"description\": \"Information about the <code>DeleteResolverEndpoint</code> request, including the status of the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-delete-resolver-endpoint-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: DeleteResolverEndpointResponse
---
