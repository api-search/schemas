---
description: Contains information about which data sources are enabled.
layout: schema
name: DataSourceConfigurations
properties_list:
- description: ''
  name: S3Logs
  type: object
- description: ''
  name: Kubernetes
  type: object
- description: ''
  name: MalwareProtection
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-data-source-configurations-schema.json
slug: guardduty-data-source-configurations
source_filename: guardduty-data-source-configurations-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-data-source-configurations-schema.json\",\n  \"title\": \"DataSourceConfigurations\",\n  \"description\": \"Contains information about which data sources are enabled.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Logs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3LogsConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"s3Logs\"\n          },\n          \"description\": \"Describes whether S3 data event logs are enabled as a data source.\"\n        }\n      ]\n    },\n    \"Kubernetes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KubernetesConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kubernetes\"\n          },\n          \"description\": \"\
  Describes whether any Kubernetes logs are enabled as data sources.\"\n        }\n      ]\n    },\n    \"MalwareProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MalwareProtectionConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"malwareProtection\"\n          },\n          \"description\": \"Describes whether Malware Protection is enabled as a data source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-data-source-configurations-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DataSourceConfigurations
---
