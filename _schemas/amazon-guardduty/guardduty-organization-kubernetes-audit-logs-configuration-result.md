---
description: The current configuration of Kubernetes audit logs as a data source for the organization.
layout: schema
name: OrganizationKubernetesAuditLogsConfigurationResult
properties_list:
- description: ''
  name: AutoEnable
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-organization-kubernetes-audit-logs-configuration-result-schema.json
slug: guardduty-organization-kubernetes-audit-logs-configuration-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-kubernetes-audit-logs-configuration-result-schema.json\",\n  \"title\": \"OrganizationKubernetesAuditLogsConfigurationResult\",\n  \"description\": \"The current configuration of Kubernetes audit logs as a data source for the organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"autoEnable\"\n          },\n          \"description\": \"Whether Kubernetes audit logs data source should be auto-enabled for new members joining the organization.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoEnable\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-kubernetes-audit-logs-configuration-result-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: OrganizationKubernetesAuditLogsConfigurationResult
---
