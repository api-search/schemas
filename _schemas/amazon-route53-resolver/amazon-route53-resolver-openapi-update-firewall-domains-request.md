---
description: UpdateFirewallDomainsRequest schema from openapi
layout: schema
name: UpdateFirewallDomainsRequest
properties_list:
- description: ''
  name: FirewallDomainListId
  type: object
- description: ''
  name: Operation
  type: object
- description: ''
  name: Domains
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-update-firewall-domains-request-schema.json
slug: amazon-route53-resolver-openapi-update-firewall-domains-request
source_filename: amazon-route53-resolver-openapi-update-firewall-domains-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-firewall-domains-request-schema.json\",\n  \"title\": \"UpdateFirewallDomainsRequest\",\n  \"description\": \"UpdateFirewallDomainsRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallDomainListId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the domain list whose domains you want to update. \"\n        }\n      ]\n    },\n    \"Operation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallDomainUpdateOperation\"\n        },\n        {\n          \"description\": \"<p>What you want DNS Firewall to do with the domains that you are providing: </p> <ul> <li> <p> <code>ADD</code>\
  \ - Add the domains to the ones that are already in the domain list. </p> </li> <li> <p> <code>REMOVE</code> - Search the domain list for the domains and remove them from the list.</p> </li> <li> <p> <code>REPLACE</code> - Update the domain list to exactly match the list that you are providing. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Domains\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallDomains\"\n        },\n        {\n          \"description\": \"<p>A list of domains to use in the update operation.</p> <important> <p>There is a limit of 1000 domains per request.</p> </important> <p>Each domain specification in your domain list must satisfy the following requirements: </p> <ul> <li> <p>It can optionally start with <code>*</code> (asterisk).</p> </li> <li> <p>With the exception of the optional starting asterisk, it must only contain the following characters: <code>A-Z</code>, <code>a-z</code>, <code>0-9</code>, <code>-</code> (hyphen).</p>\
  \ </li> <li> <p>It must be from 1-255 characters in length. </p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FirewallDomainListId\",\n    \"Operation\",\n    \"Domains\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-firewall-domains-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: UpdateFirewallDomainsRequest
---
