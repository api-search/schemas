---
description: Contains information about the free trial period for a feature.
layout: schema
name: FreeTrialFeatureConfigurationResult
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: FreeTrialDaysRemaining
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-free-trial-feature-configuration-result-schema.json
slug: guardduty-free-trial-feature-configuration-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-free-trial-feature-configuration-result-schema.json\",\n  \"title\": \"FreeTrialFeatureConfigurationResult\",\n  \"description\": \"Contains information about the free trial period for a feature.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FreeTrialFeatureResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the feature for which the free trial is configured.\"\n        }\n      ]\n    },\n    \"FreeTrialDaysRemaining\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"freeTrialDaysRemaining\"\n        \
  \  },\n          \"description\": \"The number of the remaining free trial days for the feature.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-free-trial-feature-configuration-result-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: FreeTrialFeatureConfigurationResult
---
