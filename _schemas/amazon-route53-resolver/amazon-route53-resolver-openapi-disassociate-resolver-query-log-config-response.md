---
description: DisassociateResolverQueryLogConfigResponse schema from openapi
layout: schema
name: DisassociateResolverQueryLogConfigResponse
properties_list:
- description: ''
  name: ResolverQueryLogConfigAssociation
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-disassociate-resolver-query-log-config-response-schema.json
slug: amazon-route53-resolver-openapi-disassociate-resolver-query-log-config-response
source_filename: amazon-route53-resolver-openapi-disassociate-resolver-query-log-config-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-disassociate-resolver-query-log-config-response-schema.json\",\n  \"title\": \"DisassociateResolverQueryLogConfigResponse\",\n  \"description\": \"DisassociateResolverQueryLogConfigResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverQueryLogConfigAssociation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverQueryLogConfigAssociation\"\n        },\n        {\n          \"description\": \"A complex type that contains settings for the association that you deleted between an Amazon VPC and a query logging configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-disassociate-resolver-query-log-config-response-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: DisassociateResolverQueryLogConfigResponse
---
