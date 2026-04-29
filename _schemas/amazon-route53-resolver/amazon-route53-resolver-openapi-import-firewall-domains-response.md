---
description: ImportFirewallDomainsResponse schema from openapi
layout: schema
name: ImportFirewallDomainsResponse
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-import-firewall-domains-response-schema.json
slug: amazon-route53-resolver-openapi-import-firewall-domains-response
source_filename: amazon-route53-resolver-openapi-import-firewall-domains-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-import-firewall-domains-response-schema.json\",\n  \"title\": \"ImportFirewallDomainsResponse\",\n  \"description\": \"ImportFirewallDomainsResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The Id of the firewall domain list that DNS Firewall just updated.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the domain list. \"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallDomainListStatus\"\
  \n        },\n        {\n          \"description\": \"Status of the import request.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusMessage\"\n        },\n        {\n          \"description\": \"Additional information about the status of the list, if available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-import-firewall-domains-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ImportFirewallDomainsResponse
---
