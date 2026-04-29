---
description: GetResolverEndpointRequest schema from openapi
layout: schema
name: GetResolverEndpointRequest
properties_list:
- description: ''
  name: ResolverEndpointId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-get-resolver-endpoint-request-schema.json
slug: amazon-route53-resolver-openapi-get-resolver-endpoint-request
source_filename: amazon-route53-resolver-openapi-get-resolver-endpoint-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-endpoint-request-schema.json\",\n  \"title\": \"GetResolverEndpointRequest\",\n  \"description\": \"GetResolverEndpointRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverEndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Resolver endpoint that you want to get information about.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResolverEndpointId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-endpoint-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: GetResolverEndpointRequest
---
