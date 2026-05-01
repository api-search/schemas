---
description: Information about the additional configuration for the member account.
layout: schema
name: MemberAdditionalConfiguration
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-member-additional-configuration-schema.json
slug: guardduty-member-additional-configuration
source_filename: guardduty-member-additional-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-member-additional-configuration-schema.json\",\n  \"title\": \"MemberAdditionalConfiguration\",\n  \"description\": \"Information about the additional configuration for the member account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrgFeatureAdditionalConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Name of the additional configuration.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FeatureStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"Status of the\
  \ additional configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-member-additional-configuration-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: MemberAdditionalConfiguration
---
