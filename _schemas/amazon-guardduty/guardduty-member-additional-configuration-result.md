---
description: Information about the additional configuration for the member account.
layout: schema
name: MemberAdditionalConfigurationResult
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: UpdatedAt
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-member-additional-configuration-result-schema.json
slug: guardduty-member-additional-configuration-result
source_filename: guardduty-member-additional-configuration-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-member-additional-configuration-result-schema.json\",\n  \"title\": \"MemberAdditionalConfigurationResult\",\n  \"description\": \"Information about the additional configuration for the member account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrgFeatureAdditionalConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Indicates the name of the additional configuration that is set for the member account.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FeatureStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\
  \n          },\n          \"description\": \"Indicates the status of the additional configuration that is set for the member account.\"\n        }\n      ]\n    },\n    \"UpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"updatedAt\"\n          },\n          \"description\": \"The timestamp at which the additional configuration was set for the member account. This is in UTC format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-member-additional-configuration-result-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: MemberAdditionalConfigurationResult
---
