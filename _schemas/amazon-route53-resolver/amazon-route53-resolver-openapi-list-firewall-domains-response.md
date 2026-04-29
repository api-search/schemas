---
description: ListFirewallDomainsResponse schema from openapi
layout: schema
name: ListFirewallDomainsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Domains
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-firewall-domains-response-schema.json
slug: amazon-route53-resolver-openapi-list-firewall-domains-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-firewall-domains-response-schema.json\",\n  \"title\": \"ListFirewallDomainsResponse\",\n  \"description\": \"ListFirewallDomainsResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If objects are still available for retrieval, Resolver returns this token in the response. To retrieve the next batch of objects, provide this token in your next request.\"\n        }\n      ]\n    },\n    \"Domains\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallDomains\"\n        },\n        {\n          \"description\": \"<p>A list of the domains in the\
  \ firewall domain list. </p> <p>This might be a partial list of the domains that you've defined in the domain list. For information, see <code>MaxResults</code>. </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-firewall-domains-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ListFirewallDomainsResponse
---
