---
description: UpdateMemberDetectorsRequest schema from Amazon GuardDuty API
layout: schema
name: UpdateMemberDetectorsRequest
properties_list:
- description: ''
  name: AccountIds
  type: object
- description: ''
  name: DataSources
  type: object
- description: ''
  name: Features
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-update-member-detectors-request-schema.json
slug: guardduty-update-member-detectors-request
source_filename: guardduty-update-member-detectors-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-update-member-detectors-request-schema.json\",\n  \"title\": \"UpdateMemberDetectorsRequest\",\n  \"description\": \"UpdateMemberDetectorsRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountIds\"\n          },\n          \"description\": \"A list of member account IDs to be updated.\"\n        }\n      ]\n    },\n    \"DataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceConfigurations\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"dataSources\"\n          },\n   \
  \       \"description\": \"Describes which data sources will be updated.This parameter is deprecated, use Features instead\"\n        }\n      ]\n    },\n    \"Features\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberFeaturesConfigurations\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"features\"\n          },\n          \"description\": \"A list of features that will be updated for the specified member accounts.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-update-member-detectors-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UpdateMemberDetectorsRequest
---
