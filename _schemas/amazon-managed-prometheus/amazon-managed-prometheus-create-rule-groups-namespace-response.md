---
description: Represents the output of a CreateRuleGroupsNamespace operation.
layout: schema
name: CreateRuleGroupsNamespaceResponse
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-create-rule-groups-namespace-response-schema.json
slug: amazon-managed-prometheus-create-rule-groups-namespace-response
source_filename: amazon-managed-prometheus-create-rule-groups-namespace-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-rule-groups-namespace-response-schema.json\",\n  \"title\": \"CreateRuleGroupsNamespaceResponse\",\n  \"description\": \"Represents the output of a CreateRuleGroupsNamespace operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupsNamespaceName\"\n        },\n        {\n          \"description\": \"The rule groups namespace name.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupsNamespaceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of this rule groups namespace.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/RuleGroupsNamespaceStatus\"\n        },\n        {\n          \"description\": \"The status of rule groups namespace.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags of this rule groups namespace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"arn\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-rule-groups-namespace-response-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: CreateRuleGroupsNamespaceResponse
---
