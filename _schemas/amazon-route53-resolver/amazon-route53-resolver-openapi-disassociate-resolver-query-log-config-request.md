---
description: DisassociateResolverQueryLogConfigRequest schema from openapi
layout: schema
name: DisassociateResolverQueryLogConfigRequest
properties_list:
- description: ''
  name: ResolverQueryLogConfigId
  type: object
- description: ''
  name: ResourceId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-disassociate-resolver-query-log-config-request-schema.json
slug: amazon-route53-resolver-openapi-disassociate-resolver-query-log-config-request
source_filename: amazon-route53-resolver-openapi-disassociate-resolver-query-log-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-disassociate-resolver-query-log-config-request-schema.json\",\n  \"title\": \"DisassociateResolverQueryLogConfigRequest\",\n  \"description\": \"DisassociateResolverQueryLogConfigRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverQueryLogConfigId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the query logging configuration that you want to disassociate a specified VPC from.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon VPC that you want to disassociate\
  \ from a specified query logging configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResolverQueryLogConfigId\",\n    \"ResourceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-disassociate-resolver-query-log-config-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: DisassociateResolverQueryLogConfigRequest
---
