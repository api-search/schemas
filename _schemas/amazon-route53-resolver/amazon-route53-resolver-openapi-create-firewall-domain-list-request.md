---
description: CreateFirewallDomainListRequest schema from openapi
layout: schema
name: CreateFirewallDomainListRequest
properties_list:
- description: ''
  name: CreatorRequestId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-create-firewall-domain-list-request-schema.json
slug: amazon-route53-resolver-openapi-create-firewall-domain-list-request
source_filename: amazon-route53-resolver-openapi-create-firewall-domain-list-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-create-firewall-domain-list-request-schema.json\",\n  \"title\": \"CreateFirewallDomainListRequest\",\n  \"description\": \"CreateFirewallDomainListRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatorRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatorRequestId\"\n        },\n        {\n          \"description\": \"A unique string that identifies the request and that allows you to retry failed requests without the risk of running the operation twice. <code>CreatorRequestId</code> can be any unique string, for example, a date/time stamp. \"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n  \
  \      {\n          \"description\": \"A name that lets you identify the domain list to manage and use it.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A list of the tag keys and values that you want to associate with the domain list. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CreatorRequestId\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-create-firewall-domain-list-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: CreateFirewallDomainListRequest
---
