---
description: GetFirewallConfigResponse schema from openapi
layout: schema
name: GetFirewallConfigResponse
properties_list:
- description: ''
  name: FirewallConfig
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-get-firewall-config-response-schema.json
slug: amazon-route53-resolver-openapi-get-firewall-config-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-firewall-config-response-schema.json\",\n  \"title\": \"GetFirewallConfigResponse\",\n  \"description\": \"GetFirewallConfigResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallConfig\"\n        },\n        {\n          \"description\": \"Configuration of the firewall behavior provided by DNS Firewall for a single VPC from AmazonVPC. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-firewall-config-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: GetFirewallConfigResponse
---
