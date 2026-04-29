---
description: Describes whether Kubernetes audit logs are enabled as a data source.
layout: schema
name: KubernetesAuditLogsConfiguration
properties_list:
- description: ''
  name: Enable
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-kubernetes-audit-logs-configuration-schema.json
slug: guardduty-kubernetes-audit-logs-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-audit-logs-configuration-schema.json\",\n  \"title\": \"KubernetesAuditLogsConfiguration\",\n  \"description\": \"Describes whether Kubernetes audit logs are enabled as a data source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"enable\"\n          },\n          \"description\": \"The status of Kubernetes audit logs as a data source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Enable\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-audit-logs-configuration-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: KubernetesAuditLogsConfiguration
---
