---
description: GetFindingsStatisticsRequest schema from Amazon GuardDuty API
layout: schema
name: GetFindingsStatisticsRequest
properties_list:
- description: ''
  name: FindingStatisticTypes
  type: object
- description: ''
  name: FindingCriteria
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-findings-statistics-request-schema.json
slug: guardduty-get-findings-statistics-request
source_filename: guardduty-get-findings-statistics-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-findings-statistics-request-schema.json\",\n  \"title\": \"GetFindingsStatisticsRequest\",\n  \"description\": \"GetFindingsStatisticsRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FindingStatisticTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingStatisticTypes\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"findingStatisticTypes\"\n          },\n          \"description\": \"The types of finding statistics to retrieve.\"\n        }\n      ]\n    },\n    \"FindingCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingCriteria\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"findingCriteria\"\n          },\n   \
  \       \"description\": \"Represents the criteria that is used for querying findings.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FindingStatisticTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-findings-statistics-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetFindingsStatisticsRequest
---
