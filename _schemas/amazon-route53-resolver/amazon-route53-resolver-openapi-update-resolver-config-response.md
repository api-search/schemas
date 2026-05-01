---
description: UpdateResolverConfigResponse schema from openapi
layout: schema
name: UpdateResolverConfigResponse
properties_list:
- description: ''
  name: ResolverConfig
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-update-resolver-config-response-schema.json
slug: amazon-route53-resolver-openapi-update-resolver-config-response
source_filename: amazon-route53-resolver-openapi-update-resolver-config-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-resolver-config-response-schema.json\",\n  \"title\": \"UpdateResolverConfigResponse\",\n  \"description\": \"UpdateResolverConfigResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverConfig\"\n        },\n        {\n          \"description\": \"An array that contains settings for the specified Resolver configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-resolver-config-response-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: UpdateResolverConfigResponse
---
