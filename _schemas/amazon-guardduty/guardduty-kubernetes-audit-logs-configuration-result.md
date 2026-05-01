---
description: Describes whether Kubernetes audit logs are enabled as a data source.
layout: schema
name: KubernetesAuditLogsConfigurationResult
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-kubernetes-audit-logs-configuration-result-schema.json
slug: guardduty-kubernetes-audit-logs-configuration-result
source_filename: guardduty-kubernetes-audit-logs-configuration-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-audit-logs-configuration-result-schema.json\",\n  \"title\": \"KubernetesAuditLogsConfigurationResult\",\n  \"description\": \"Describes whether Kubernetes audit logs are enabled as a data source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"A value that describes whether Kubernetes audit logs are enabled as a data source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-audit-logs-configuration-result-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: KubernetesAuditLogsConfigurationResult
---
