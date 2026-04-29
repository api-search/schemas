---
description: ListFirewallsRequest schema from Amazon Network Firewall
layout: schema
name: ListFirewallsRequest
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: VpcIds
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-list-firewalls-request-schema.json
slug: openapi-list-firewalls-request
source_filename: openapi-list-firewalls-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-list-firewalls-request-schema.json\",\n  \"title\": \"ListFirewallsRequest\",\n  \"description\": \"ListFirewallsRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"When you request a list of objects with a <code>MaxResults</code> setting, if the number of objects that are still available for retrieval exceeds the maximum you requested, Network Firewall returns a <code>NextToken</code> value in the response. To retrieve the next batch of objects, use the token returned from the prior request in your next request.\"\n        }\n      ]\n    },\n    \"VpcIds\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/VpcIds\"\n        },\n        {\n          \"description\": \"The unique identifiers of the VPCs that you want Network Firewall to retrieve the firewalls for. Leave this blank to retrieve all firewalls that you have defined.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationMaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of objects that you want Network Firewall to return for this request. If more objects are available, in the response, Network Firewall provides a <code>NextToken</code> value that you can use in a subsequent call to get the next batch of objects.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-list-firewalls-request-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: ListFirewallsRequest
---
