---
description: Contains information about the features for the member account.
layout: schema
name: MemberFeaturesConfiguration
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
schema_file: json-schema/guardduty-member-features-configuration-schema.json
slug: guardduty-member-features-configuration
source_filename: guardduty-member-features-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-member-features-configuration-schema.json\",\n  \"title\": \"MemberFeaturesConfiguration\",\n  \"description\": \"Contains information about the features for the member account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrgFeature\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the feature.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FeatureStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"The status of the feature.\"\n        }\n      ]\n    },\n  \
  \  \"AdditionalConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberAdditionalConfigurations\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"additionalConfiguration\"\n          },\n          \"description\": \"Additional configuration of the feature for the member account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-member-features-configuration-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: MemberFeaturesConfiguration
---
