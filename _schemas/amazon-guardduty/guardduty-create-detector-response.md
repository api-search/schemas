---
description: CreateDetectorResponse schema from Amazon GuardDuty API
layout: schema
name: CreateDetectorResponse
properties_list:
- description: ''
  name: DetectorId
  type: object
- description: ''
  name: UnprocessedDataSources
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-create-detector-response-schema.json
slug: guardduty-create-detector-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-detector-response-schema.json\",\n  \"title\": \"CreateDetectorResponse\",\n  \"description\": \"CreateDetectorResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DetectorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"detectorId\"\n          },\n          \"description\": \"The unique ID of the created detector.\"\n        }\n      ]\n    },\n    \"UnprocessedDataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnprocessedDataSourcesResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"unprocessedDataSources\"\n          },\n          \"description\": \"Specifies\
  \ the data sources that couldn't be enabled when GuardDuty was enabled for the first time.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-detector-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CreateDetectorResponse
---
