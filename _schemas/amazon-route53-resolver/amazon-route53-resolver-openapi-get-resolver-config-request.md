---
description: GetResolverConfigRequest schema from openapi
layout: schema
name: GetResolverConfigRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-get-resolver-config-request-schema.json
slug: amazon-route53-resolver-openapi-get-resolver-config-request
source_filename: amazon-route53-resolver-openapi-get-resolver-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-config-request-schema.json\",\n  \"title\": \"GetResolverConfigRequest\",\n  \"description\": \"GetResolverConfigRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"Resource ID of the Amazon VPC that you want to get information about.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-config-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: GetResolverConfigRequest
---
