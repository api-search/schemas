---
description: ImportFirewallDomainsRequest schema from openapi
layout: schema
name: ImportFirewallDomainsRequest
properties_list:
- description: ''
  name: FirewallDomainListId
  type: object
- description: ''
  name: Operation
  type: object
- description: ''
  name: DomainFileUrl
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-import-firewall-domains-request-schema.json
slug: amazon-route53-resolver-openapi-import-firewall-domains-request
source_filename: amazon-route53-resolver-openapi-import-firewall-domains-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-import-firewall-domains-request-schema.json\",\n  \"title\": \"ImportFirewallDomainsRequest\",\n  \"description\": \"ImportFirewallDomainsRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallDomainListId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the domain list that you want to modify with the import operation.\"\n        }\n      ]\n    },\n    \"Operation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallDomainImportOperation\"\n        },\n        {\n          \"description\": \"What you want DNS Firewall to do with the domains that are listed in the file. This must be set\
  \ to <code>REPLACE</code>, which updates the domain list to exactly match the list in the file. \"\n        }\n      ]\n    },\n    \"DomainFileUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainListFileUrl\"\n        },\n        {\n          \"description\": \"<p>The fully qualified URL or URI of the file stored in Amazon Simple Storage Service (Amazon S3) that contains the list of domains to import.</p> <p>The file must be in an S3 bucket that's in the same Region as your DNS Firewall. The file must be a text file and must contain a single domain per line.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FirewallDomainListId\",\n    \"Operation\",\n    \"DomainFileUrl\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-import-firewall-domains-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: ImportFirewallDomainsRequest
---
