---
description: Organization-wide Kubernetes audit logs configuration.
layout: schema
name: OrganizationKubernetesAuditLogsConfiguration
properties_list:
- description: ''
  name: AutoEnable
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-organization-kubernetes-audit-logs-configuration-schema.json
slug: guardduty-organization-kubernetes-audit-logs-configuration
source_filename: guardduty-organization-kubernetes-audit-logs-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-kubernetes-audit-logs-configuration-schema.json\",\n  \"title\": \"OrganizationKubernetesAuditLogsConfiguration\",\n  \"description\": \"Organization-wide Kubernetes audit logs configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"autoEnable\"\n          },\n          \"description\": \"A value that contains information on whether Kubernetes audit logs should be enabled automatically as a data source for the organization.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoEnable\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-kubernetes-audit-logs-configuration-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: OrganizationKubernetesAuditLogsConfiguration
---
