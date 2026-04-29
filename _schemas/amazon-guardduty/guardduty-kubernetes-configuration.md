---
description: Describes whether any Kubernetes data sources are enabled.
layout: schema
name: KubernetesConfiguration
properties_list:
- description: ''
  name: AuditLogs
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-kubernetes-configuration-schema.json
slug: guardduty-kubernetes-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-configuration-schema.json\",\n  \"title\": \"KubernetesConfiguration\",\n  \"description\": \"Describes whether any Kubernetes data sources are enabled.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuditLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KubernetesAuditLogsConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"auditLogs\"\n          },\n          \"description\": \"The status of Kubernetes audit logs as a data source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AuditLogs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-configuration-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: KubernetesConfiguration
---
