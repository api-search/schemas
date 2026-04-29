---
description: The current configuration of all Kubernetes data sources for the organization.
layout: schema
name: OrganizationKubernetesConfigurationResult
properties_list:
- description: ''
  name: AuditLogs
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-organization-kubernetes-configuration-result-schema.json
slug: guardduty-organization-kubernetes-configuration-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-kubernetes-configuration-result-schema.json\",\n  \"title\": \"OrganizationKubernetesConfigurationResult\",\n  \"description\": \"The current configuration of all Kubernetes data sources for the organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuditLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationKubernetesAuditLogsConfigurationResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"auditLogs\"\n          },\n          \"description\": \"The current configuration of Kubernetes audit logs as a data source for the organization.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AuditLogs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-kubernetes-configuration-result-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: OrganizationKubernetesConfigurationResult
---
