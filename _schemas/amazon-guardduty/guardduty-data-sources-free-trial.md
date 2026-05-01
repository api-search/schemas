---
description: Contains information about which data sources are enabled for the GuardDuty member account.
layout: schema
name: DataSourcesFreeTrial
properties_list:
- description: ''
  name: CloudTrail
  type: object
- description: ''
  name: DnsLogs
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
schema_file: json-schema/guardduty-data-sources-free-trial-schema.json
slug: guardduty-data-sources-free-trial
source_filename: guardduty-data-sources-free-trial-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-data-sources-free-trial-schema.json\",\n  \"title\": \"DataSourcesFreeTrial\",\n  \"description\": \"Contains information about which data sources are enabled for the GuardDuty member account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CloudTrail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceFreeTrial\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cloudTrail\"\n          },\n          \"description\": \"Describes whether any Amazon Web Services CloudTrail management event logs are enabled as data sources.\"\n        }\n      ]\n    },\n    \"DnsLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceFreeTrial\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"dnsLogs\"\n          },\n          \"description\": \"Describes whether any DNS logs are enabled as data sources.\"\n        }\n      ]\n    },\n    \"FlowLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceFreeTrial\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowLogs\"\n          },\n          \"description\": \"Describes whether any VPC Flow logs are enabled as data sources.\"\n        }\n      ]\n    },\n    \"S3Logs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceFreeTrial\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"s3Logs\"\n          },\n          \"description\": \"Describes whether any S3 data event logs are enabled as data sources.\"\n        }\n      ]\n    },\n    \"Kubernetes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KubernetesDataSourceFreeTrial\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"kubernetes\"\n          },\n          \"description\": \"Describes whether any Kubernetes logs are enabled as data sources.\"\n        }\n      ]\n    },\n    \"MalwareProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MalwareProtectionDataSourceFreeTrial\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"malwareProtection\"\n          },\n          \"description\": \"Describes whether Malware Protection is enabled as a data source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-data-sources-free-trial-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DataSourcesFreeTrial
---
