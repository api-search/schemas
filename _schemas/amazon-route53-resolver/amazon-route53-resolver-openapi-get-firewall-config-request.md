---
description: GetFirewallConfigRequest schema from openapi
layout: schema
name: GetFirewallConfigRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-get-firewall-config-request-schema.json
slug: amazon-route53-resolver-openapi-get-firewall-config-request
source_filename: amazon-route53-resolver-openapi-get-firewall-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-firewall-config-request-schema.json\",\n  \"title\": \"GetFirewallConfigRequest\",\n  \"description\": \"GetFirewallConfigRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the VPC from Amazon VPC that the configuration is for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-firewall-config-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: GetFirewallConfigRequest
---
