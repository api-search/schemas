---
description: Organization-wide Kubernetes data sources configurations.
layout: schema
name: OrganizationKubernetesConfiguration
properties_list:
- description: ''
  name: AuditLogs
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-organization-kubernetes-configuration-schema.json
slug: guardduty-organization-kubernetes-configuration
source_filename: guardduty-organization-kubernetes-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-kubernetes-configuration-schema.json\",\n  \"title\": \"OrganizationKubernetesConfiguration\",\n  \"description\": \"Organization-wide Kubernetes data sources configurations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuditLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationKubernetesAuditLogsConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"auditLogs\"\n          },\n          \"description\": \"Whether Kubernetes audit logs data source should be auto-enabled for new members joining the organization.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AuditLogs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-kubernetes-configuration-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: OrganizationKubernetesConfiguration
---
