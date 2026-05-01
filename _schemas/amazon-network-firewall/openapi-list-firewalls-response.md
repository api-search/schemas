---
description: ListFirewallsResponse schema from Amazon Network Firewall
layout: schema
name: ListFirewallsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Firewalls
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-list-firewalls-response-schema.json
slug: openapi-list-firewalls-response
source_filename: openapi-list-firewalls-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-list-firewalls-response-schema.json\",\n  \"title\": \"ListFirewallsResponse\",\n  \"description\": \"ListFirewallsResponse schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"When you request a list of objects with a <code>MaxResults</code> setting, if the number of objects that are still available for retrieval exceeds the maximum you requested, Network Firewall returns a <code>NextToken</code> value in the response. To retrieve the next batch of objects, use the token returned from the prior request in your next request.\"\n        }\n      ]\n    },\n    \"Firewalls\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/Firewalls\"\n        },\n        {\n          \"description\": \"The firewall metadata objects for the VPCs that you specified. Depending on your setting for max results and the number of firewalls you have, a single call might not be the full list. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-list-firewalls-response-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: ListFirewallsResponse
---
