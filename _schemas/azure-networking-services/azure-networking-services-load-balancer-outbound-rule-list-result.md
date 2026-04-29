---
description: Response for ListOutboundRule API service call.
layout: schema
name: LoadBalancerOutboundRuleListResult
properties_list:
- description: The URL to get the next set of results.
  name: nextLink
  type: string
- description: A list of outbound rules in a load balancer.
  name: value
  type: array
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-load-balancer-outbound-rule-list-result-schema.json
slug: azure-networking-services-load-balancer-outbound-rule-list-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-load-balancer-outbound-rule-list-result-schema.json\",\n  \"title\": \"LoadBalancerOutboundRuleListResult\",\n  \"description\": \"Response for ListOutboundRule API service call.\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"The URL to get the next set of results.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"A list of outbound rules in a load balancer.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/OutboundRule\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-load-balancer-outbound-rule-list-result-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: LoadBalancerOutboundRuleListResult
---
