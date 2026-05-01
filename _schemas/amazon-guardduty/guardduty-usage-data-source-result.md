---
description: Contains information on the result of usage based on data source type.
layout: schema
name: UsageDataSourceResult
properties_list:
- description: ''
  name: DataSource
  type: object
- description: ''
  name: Total
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-usage-data-source-result-schema.json
slug: guardduty-usage-data-source-result
source_filename: guardduty-usage-data-source-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-usage-data-source-result-schema.json\",\n  \"title\": \"UsageDataSourceResult\",\n  \"description\": \"Contains information on the result of usage based on data source type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DataSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dataSource\"\n          },\n          \"description\": \"The data source type that generated usage.\"\n        }\n      ]\n    },\n    \"Total\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Total\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"total\"\n          },\n          \"description\": \"Represents the total of usage for the specified\
  \ data source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-usage-data-source-result-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UsageDataSourceResult
---
