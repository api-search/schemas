---
description: Contains information about which data sources are enabled for the GuardDuty member account.
layout: schema
name: DataSourceFreeTrial
properties_list:
- description: ''
  name: FreeTrialDaysRemaining
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-data-source-free-trial-schema.json
slug: guardduty-data-source-free-trial
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-data-source-free-trial-schema.json\",\n  \"title\": \"DataSourceFreeTrial\",\n  \"description\": \"Contains information about which data sources are enabled for the GuardDuty member account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FreeTrialDaysRemaining\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"freeTrialDaysRemaining\"\n          },\n          \"description\": \"A value that specifies the number of days left to use each enabled data source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-data-source-free-trial-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DataSourceFreeTrial
---
