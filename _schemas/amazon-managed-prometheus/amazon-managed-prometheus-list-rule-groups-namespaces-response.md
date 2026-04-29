---
description: Represents the output of a ListRuleGroupsNamespaces operation.
layout: schema
name: ListRuleGroupsNamespacesResponse
properties_list:
- description: ''
  name: ruleGroupsNamespaces
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-list-rule-groups-namespaces-response-schema.json
slug: amazon-managed-prometheus-list-rule-groups-namespaces-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-list-rule-groups-namespaces-response-schema.json\",\n  \"title\": \"ListRuleGroupsNamespacesResponse\",\n  \"description\": \"Represents the output of a ListRuleGroupsNamespaces operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ruleGroupsNamespaces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupsNamespaceSummaryList\"\n        },\n        {\n          \"description\": \"The list of the selected rule groups namespaces.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Pagination token to use when requesting the next page in this list.\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"ruleGroupsNamespaces\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-list-rule-groups-namespaces-response-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: ListRuleGroupsNamespacesResponse
---
