---
description: Represents the input of a CreateRuleGroupsNamespace operation.
layout: schema
name: CreateRuleGroupsNamespaceRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: data
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-create-rule-groups-namespace-request-schema.json
slug: amazon-managed-prometheus-create-rule-groups-namespace-request
source_filename: amazon-managed-prometheus-create-rule-groups-namespace-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-rule-groups-namespace-request-schema.json\",\n  \"title\": \"CreateRuleGroupsNamespaceRequest\",\n  \"description\": \"Represents the input of a CreateRuleGroupsNamespace operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupsNamespaceName\"\n        },\n        {\n          \"description\": \"The rule groups namespace name.\"\n        }\n      ]\n    },\n    \"data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupsNamespaceData\"\n        },\n        {\n          \"description\": \"The namespace data that define the rule groups.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/IdempotencyToken\"\n        },\n        {\n          \"description\": \"Optional, unique, case-sensitive, user-provided identifier to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Optional, user-provided tags for this rule groups namespace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-rule-groups-namespace-request-schema.json
tags:
- Containers
- Monitoring
- Observability
- Prometheus
title: CreateRuleGroupsNamespaceRequest
---
