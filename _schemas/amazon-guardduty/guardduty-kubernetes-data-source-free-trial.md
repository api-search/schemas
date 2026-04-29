---
description: Provides details about the Kubernetes resources when it is enabled as a data source.
layout: schema
name: KubernetesDataSourceFreeTrial
properties_list:
- description: ''
  name: AuditLogs
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-kubernetes-data-source-free-trial-schema.json
slug: guardduty-kubernetes-data-source-free-trial
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-data-source-free-trial-schema.json\",\n  \"title\": \"KubernetesDataSourceFreeTrial\",\n  \"description\": \"Provides details about the Kubernetes resources when it is enabled as a data source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuditLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceFreeTrial\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"auditLogs\"\n          },\n          \"description\": \"Describes whether Kubernetes audit logs are enabled as a data source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-data-source-free-trial-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: KubernetesDataSourceFreeTrial
---
