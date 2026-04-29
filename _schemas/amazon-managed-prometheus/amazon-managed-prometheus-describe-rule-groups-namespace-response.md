---
description: Represents the output of a DescribeRuleGroupsNamespace operation.
layout: schema
name: DescribeRuleGroupsNamespaceResponse
properties_list:
- description: ''
  name: ruleGroupsNamespace
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-describe-rule-groups-namespace-response-schema.json
slug: amazon-managed-prometheus-describe-rule-groups-namespace-response
source_filename: amazon-managed-prometheus-describe-rule-groups-namespace-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-describe-rule-groups-namespace-response-schema.json\",\n  \"title\": \"DescribeRuleGroupsNamespaceResponse\",\n  \"description\": \"Represents the output of a DescribeRuleGroupsNamespace operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ruleGroupsNamespace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupsNamespaceDescription\"\n        },\n        {\n          \"description\": \"The selected rule groups namespace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ruleGroupsNamespace\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-describe-rule-groups-namespace-response-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: DescribeRuleGroupsNamespaceResponse
---
