---
description: Describes whether any Kubernetes logs will be enabled as a data source.
layout: schema
name: KubernetesConfigurationResult
properties_list:
- description: ''
  name: AuditLogs
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-kubernetes-configuration-result-schema.json
slug: guardduty-kubernetes-configuration-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-configuration-result-schema.json\",\n  \"title\": \"KubernetesConfigurationResult\",\n  \"description\": \"Describes whether any Kubernetes logs will be enabled as a data source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuditLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KubernetesAuditLogsConfigurationResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"auditLogs\"\n          },\n          \"description\": \"Describes whether Kubernetes audit logs are enabled as a data source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AuditLogs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-configuration-result-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: KubernetesConfigurationResult
---
