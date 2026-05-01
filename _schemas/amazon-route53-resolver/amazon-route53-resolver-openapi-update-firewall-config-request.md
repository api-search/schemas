---
description: UpdateFirewallConfigRequest schema from openapi
layout: schema
name: UpdateFirewallConfigRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: FirewallFailOpen
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-update-firewall-config-request-schema.json
slug: amazon-route53-resolver-openapi-update-firewall-config-request
source_filename: amazon-route53-resolver-openapi-update-firewall-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-firewall-config-request-schema.json\",\n  \"title\": \"UpdateFirewallConfigRequest\",\n  \"description\": \"UpdateFirewallConfigRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the VPC that the configuration is for.\"\n        }\n      ]\n    },\n    \"FirewallFailOpen\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallFailOpenStatus\"\n        },\n        {\n          \"description\": \"<p>Determines how Route 53 Resolver handles queries during failures, for example when all traffic that is sent to DNS Firewall fails to\
  \ receive a reply. </p> <ul> <li> <p>By default, fail open is disabled, which means the failure mode is closed. This approach favors security over availability. DNS Firewall blocks queries that it is unable to evaluate properly. </p> </li> <li> <p>If you enable this option, the failure mode is open. This approach favors availability over security. DNS Firewall allows queries to proceed if it is unable to properly evaluate them. </p> </li> </ul> <p>This behavior is only enforced for VPCs that have at least one DNS Firewall rule group association. </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceId\",\n    \"FirewallFailOpen\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-firewall-config-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: UpdateFirewallConfigRequest
---
