---
description: GetResolverDnssecConfigRequest schema from openapi
layout: schema
name: GetResolverDnssecConfigRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-get-resolver-dnssec-config-request-schema.json
slug: amazon-route53-resolver-openapi-get-resolver-dnssec-config-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-dnssec-config-request-schema.json\",\n  \"title\": \"GetResolverDnssecConfigRequest\",\n  \"description\": \"GetResolverDnssecConfigRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the virtual private cloud (VPC) for the DNSSEC validation status.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-dnssec-config-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: GetResolverDnssecConfigRequest
---
