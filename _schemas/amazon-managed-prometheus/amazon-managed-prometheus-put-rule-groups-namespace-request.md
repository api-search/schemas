---
description: Represents the input of a PutRuleGroupsNamespace operation.
layout: schema
name: PutRuleGroupsNamespaceRequest
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-put-rule-groups-namespace-request-schema.json
slug: amazon-managed-prometheus-put-rule-groups-namespace-request
source_filename: amazon-managed-prometheus-put-rule-groups-namespace-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-put-rule-groups-namespace-request-schema.json\",\n  \"title\": \"PutRuleGroupsNamespaceRequest\",\n  \"description\": \"Represents the input of a PutRuleGroupsNamespace operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupsNamespaceData\"\n        },\n        {\n          \"description\": \"The namespace data that define the rule groups.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyToken\"\n        },\n        {\n          \"description\": \"Optional, unique, case-sensitive, user-provided identifier to ensure the idempotency of the request.\"\n        }\n      ]\n   \
  \ }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-put-rule-groups-namespace-request-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: PutRuleGroupsNamespaceRequest
---
