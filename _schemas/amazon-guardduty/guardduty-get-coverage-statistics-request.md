---
description: GetCoverageStatisticsRequest schema from Amazon GuardDuty API
layout: schema
name: GetCoverageStatisticsRequest
properties_list:
- description: ''
  name: FilterCriteria
  type: object
- description: ''
  name: StatisticsType
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-coverage-statistics-request-schema.json
slug: guardduty-get-coverage-statistics-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-coverage-statistics-request-schema.json\",\n  \"title\": \"GetCoverageStatisticsRequest\",\n  \"description\": \"GetCoverageStatisticsRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FilterCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageFilterCriteria\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filterCriteria\"\n          },\n          \"description\": \"Represents the criteria used to filter the coverage statistics\"\n        }\n      ]\n    },\n    \"StatisticsType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageStatisticsTypeList\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"statisticsType\"\n   \
  \       },\n          \"description\": \"Represents the statistics type used to aggregate the coverage details.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"StatisticsType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-coverage-statistics-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetCoverageStatisticsRequest
---
