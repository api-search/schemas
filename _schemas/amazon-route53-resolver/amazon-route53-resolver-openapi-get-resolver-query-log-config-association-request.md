---
description: GetResolverQueryLogConfigAssociationRequest schema from openapi
layout: schema
name: GetResolverQueryLogConfigAssociationRequest
properties_list:
- description: ''
  name: ResolverQueryLogConfigAssociationId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-get-resolver-query-log-config-association-request-schema.json
slug: amazon-route53-resolver-openapi-get-resolver-query-log-config-association-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-query-log-config-association-request-schema.json\",\n  \"title\": \"GetResolverQueryLogConfigAssociationRequest\",\n  \"description\": \"GetResolverQueryLogConfigAssociationRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverQueryLogConfigAssociationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Resolver query logging configuration association that you want to get information about.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResolverQueryLogConfigAssociationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-query-log-config-association-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: GetResolverQueryLogConfigAssociationRequest
---
