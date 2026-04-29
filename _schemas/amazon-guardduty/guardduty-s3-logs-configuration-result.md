---
description: Describes whether S3 data event logs will be enabled as a data source.
layout: schema
name: S3LogsConfigurationResult
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-s3-logs-configuration-result-schema.json
slug: guardduty-s3-logs-configuration-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-s3-logs-configuration-result-schema.json\",\n  \"title\": \"S3LogsConfigurationResult\",\n  \"description\": \"Describes whether S3 data event logs will be enabled as a data source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"A value that describes whether S3 data event logs are automatically enabled for new members of the organization.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-s3-logs-configuration-result-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: S3LogsConfigurationResult
---
