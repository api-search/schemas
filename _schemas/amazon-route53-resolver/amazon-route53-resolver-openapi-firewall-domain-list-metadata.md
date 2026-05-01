---
description: <p>Minimal high-level information for a firewall domain list. The action <a>ListFirewallDomainLists</a> returns an array of these objects. </p> <p>To retrieve full information for a firewall domain list, call <a>GetFirewallDomainList</a> and <a>ListFirewallDomains</a>.</p>
layout: schema
name: FirewallDomainListMetadata
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: CreatorRequestId
  type: object
- description: ''
  name: ManagedOwnerName
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-firewall-domain-list-metadata-schema.json
slug: amazon-route53-resolver-openapi-firewall-domain-list-metadata
source_filename: amazon-route53-resolver-openapi-firewall-domain-list-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-firewall-domain-list-metadata-schema.json\",\n  \"title\": \"FirewallDomainListMetadata\",\n  \"description\": \"<p>Minimal high-level information for a firewall domain list. The action <a>ListFirewallDomainLists</a> returns an array of these objects. </p> <p>To retrieve full information for a firewall domain list, call <a>GetFirewallDomainList</a> and <a>ListFirewallDomains</a>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the domain list. \"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n \
  \         \"description\": \"The Amazon Resource Name (ARN) of the firewall domain list metadata.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the domain list. \"\n        }\n      ]\n    },\n    \"CreatorRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatorRequestId\"\n        },\n        {\n          \"description\": \"A unique string defined by you to identify the request. This allows you to retry failed requests without the risk of running the operation twice. This can be any unique string, for example, a timestamp. \"\n        }\n      ]\n    },\n    \"ManagedOwnerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServicePrinciple\"\n        },\n        {\n          \"description\": \"The owner of the list, used only for lists that are not managed by you. For\
  \ example, the managed domain list <code>AWSManagedDomainsMalwareDomainList</code> has the managed owner name <code>Route 53 Resolver DNS Firewall</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-firewall-domain-list-metadata-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: FirewallDomainListMetadata
---
