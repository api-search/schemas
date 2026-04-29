---
description: Represents a summary of the rule groups namespace.
layout: schema
name: RuleGroupsNamespaceSummary
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: modifiedAt
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-rule-groups-namespace-summary-schema.json
slug: amazon-managed-prometheus-rule-groups-namespace-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-rule-groups-namespace-summary-schema.json\",\n  \"title\": \"RuleGroupsNamespaceSummary\",\n  \"description\": \"Represents a summary of the rule groups namespace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupsNamespaceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of this rule groups namespace.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupsNamespaceName\"\n        },\n        {\n          \"description\": \"The rule groups namespace name.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/RuleGroupsNamespaceStatus\"\n        },\n        {\n          \"description\": \"The status of rule groups namespace.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the rule groups namespace was created.\"\n        }\n      ]\n    },\n    \"modifiedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the rule groups namespace was modified.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags of this rule groups namespace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"name\",\n    \"status\",\n    \"createdAt\",\n    \"modifiedAt\"\n\
  \  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-rule-groups-namespace-summary-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: RuleGroupsNamespaceSummary
---
