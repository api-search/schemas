---
description: Contains information about a GuardDuty feature.
layout: schema
name: DetectorFeatureConfiguration
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: AdditionalConfiguration
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-detector-feature-configuration-schema.json
slug: guardduty-detector-feature-configuration
source_filename: guardduty-detector-feature-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-detector-feature-configuration-schema.json\",\n  \"title\": \"DetectorFeatureConfiguration\",\n  \"description\": \"Contains information about a GuardDuty feature.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorFeature\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the feature.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FeatureStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"The status of the feature.\"\n        }\n      ]\n    },\n    \"AdditionalConfiguration\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorAdditionalConfigurations\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"additionalConfiguration\"\n          },\n          \"description\": \"Additional configuration for a resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-detector-feature-configuration-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DetectorFeatureConfiguration
---
