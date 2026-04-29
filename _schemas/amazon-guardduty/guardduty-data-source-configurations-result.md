---
description: Contains information on the status of data sources for the detector.
layout: schema
name: DataSourceConfigurationsResult
properties_list:
- description: ''
  name: CloudTrail
  type: object
- description: ''
  name: DNSLogs
  type: object
- description: ''
  name: FlowLogs
  type: object
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
schema_file: json-schema/guardduty-data-source-configurations-result-schema.json
slug: guardduty-data-source-configurations-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-data-source-configurations-result-schema.json\",\n  \"title\": \"DataSourceConfigurationsResult\",\n  \"description\": \"Contains information on the status of data sources for the detector.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CloudTrail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudTrailConfigurationResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cloudTrail\"\n          },\n          \"description\": \"An object that contains information on the status of CloudTrail as a data source.\"\n        }\n      ]\n    },\n    \"DNSLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DNSLogsConfigurationResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"\
  dnsLogs\"\n          },\n          \"description\": \"An object that contains information on the status of DNS logs as a data source.\"\n        }\n      ]\n    },\n    \"FlowLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlowLogsConfigurationResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowLogs\"\n          },\n          \"description\": \"An object that contains information on the status of VPC flow logs as a data source.\"\n        }\n      ]\n    },\n    \"S3Logs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3LogsConfigurationResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"s3Logs\"\n          },\n          \"description\": \"An object that contains information on the status of S3 Data event logs as a data source.\"\n        }\n      ]\n    },\n    \"Kubernetes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KubernetesConfigurationResult\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"kubernetes\"\n          },\n          \"description\": \"An object that contains information on the status of all Kubernetes data sources.\"\n        }\n      ]\n    },\n    \"MalwareProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MalwareProtectionConfigurationResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"malwareProtection\"\n          },\n          \"description\": \"Describes the configuration of Malware Protection data sources.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CloudTrail\",\n    \"DNSLogs\",\n    \"FlowLogs\",\n    \"S3Logs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-data-source-configurations-result-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DataSourceConfigurationsResult
---
