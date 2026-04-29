---
description: GetResolverDnssecConfigResponse schema from openapi
layout: schema
name: GetResolverDnssecConfigResponse
properties_list:
- description: ''
  name: ResolverDNSSECConfig
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-get-resolver-dnssec-config-response-schema.json
slug: amazon-route53-resolver-openapi-get-resolver-dnssec-config-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-dnssec-config-response-schema.json\",\n  \"title\": \"GetResolverDnssecConfigResponse\",\n  \"description\": \"GetResolverDnssecConfigResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolverDNSSECConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverDnssecConfig\"\n        },\n        {\n          \"description\": \"The information about a configuration for DNSSEC validation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-resolver-dnssec-config-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: GetResolverDnssecConfigResponse
---
