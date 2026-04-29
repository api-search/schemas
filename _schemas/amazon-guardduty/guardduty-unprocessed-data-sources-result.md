---
description: Specifies the names of the data sources that couldn't be enabled.
layout: schema
name: UnprocessedDataSourcesResult
properties_list:
- description: ''
  name: MalwareProtection
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-unprocessed-data-sources-result-schema.json
slug: guardduty-unprocessed-data-sources-result
source_filename: guardduty-unprocessed-data-sources-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-unprocessed-data-sources-result-schema.json\",\n  \"title\": \"UnprocessedDataSourcesResult\",\n  \"description\": \"Specifies the names of the data sources that couldn't be enabled.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MalwareProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MalwareProtectionConfigurationResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"malwareProtection\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-unprocessed-data-sources-result-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UnprocessedDataSourcesResult
---
