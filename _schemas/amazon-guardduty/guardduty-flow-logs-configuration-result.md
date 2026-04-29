---
description: Contains information on the status of VPC flow logs as a data source.
layout: schema
name: FlowLogsConfigurationResult
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-flow-logs-configuration-result-schema.json
slug: guardduty-flow-logs-configuration-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-flow-logs-configuration-result-schema.json\",\n  \"title\": \"FlowLogsConfigurationResult\",\n  \"description\": \"Contains information on the status of VPC flow logs as a data source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"Denotes whether VPC flow logs is enabled as a data source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-flow-logs-configuration-result-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: FlowLogsConfigurationResult
---
