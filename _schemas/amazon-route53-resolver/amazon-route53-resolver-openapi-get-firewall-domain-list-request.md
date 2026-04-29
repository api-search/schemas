---
description: GetFirewallDomainListRequest schema from openapi
layout: schema
name: GetFirewallDomainListRequest
properties_list:
- description: ''
  name: FirewallDomainListId
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-get-firewall-domain-list-request-schema.json
slug: amazon-route53-resolver-openapi-get-firewall-domain-list-request
source_filename: amazon-route53-resolver-openapi-get-firewall-domain-list-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-firewall-domain-list-request-schema.json\",\n  \"title\": \"GetFirewallDomainListRequest\",\n  \"description\": \"GetFirewallDomainListRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallDomainListId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the domain list. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FirewallDomainListId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-get-firewall-domain-list-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: GetFirewallDomainListRequest
---
