---
description: Contains information on the status of DNS logs as a data source.
layout: schema
name: DNSLogsConfigurationResult
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-dns-logs-configuration-result-schema.json
slug: guardduty-dns-logs-configuration-result
source_filename: guardduty-dns-logs-configuration-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-dns-logs-configuration-result-schema.json\",\n  \"title\": \"DNSLogsConfigurationResult\",\n  \"description\": \"Contains information on the status of DNS logs as a data source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"Denotes whether DNS logs is enabled as a data source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-dns-logs-configuration-result-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DNSLogsConfigurationResult
---
