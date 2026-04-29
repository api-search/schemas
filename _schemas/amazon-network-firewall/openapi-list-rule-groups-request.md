---
description: ListRuleGroupsRequest schema from Amazon Network Firewall
layout: schema
name: ListRuleGroupsRequest
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: Scope
  type: object
- description: ''
  name: ManagedType
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-list-rule-groups-request-schema.json
slug: openapi-list-rule-groups-request
source_filename: openapi-list-rule-groups-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-list-rule-groups-request-schema.json\",\n  \"title\": \"ListRuleGroupsRequest\",\n  \"description\": \"ListRuleGroupsRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"When you request a list of objects with a <code>MaxResults</code> setting, if the number of objects that are still available for retrieval exceeds the maximum you requested, Network Firewall returns a <code>NextToken</code> value in the response. To retrieve the next batch of objects, use the token returned from the prior request in your next request.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/PaginationMaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of objects that you want Network Firewall to return for this request. If more objects are available, in the response, Network Firewall provides a <code>NextToken</code> value that you can use in a subsequent call to get the next batch of objects.\"\n        }\n      ]\n    },\n    \"Scope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceManagedStatus\"\n        },\n        {\n          \"description\": \"The scope of the request. The default setting of <code>ACCOUNT</code> or a setting of <code>NULL</code> returns all of the rule groups in your account. A setting of <code>MANAGED</code> returns all available managed rule groups.\"\n        }\n      ]\n    },\n    \"ManagedType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceManagedType\"\n        },\n     \
  \   {\n          \"description\": \"Indicates the general category of the Amazon Web Services managed rule group.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupType\"\n        },\n        {\n          \"description\": \"Indicates whether the rule group is stateless or stateful. If the rule group is stateless, it contains stateless rules. If it is stateful, it contains stateful rules.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-list-rule-groups-request-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: ListRuleGroupsRequest
---
