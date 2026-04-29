---
description: Represents a condition that when matched will be added to the response of the operation.
layout: schema
name: CoverageFilterCriterion
properties_list:
- description: ''
  name: CriterionKey
  type: object
- description: ''
  name: FilterCondition
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-coverage-filter-criterion-schema.json
slug: guardduty-coverage-filter-criterion
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-filter-criterion-schema.json\",\n  \"title\": \"CoverageFilterCriterion\",\n  \"description\": \"Represents a condition that when matched will be added to the response of the operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CriterionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageFilterCriterionKey\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"criterionKey\"\n          },\n          \"description\": \"An enum value representing possible filter fields.\"\n        }\n      ]\n    },\n    \"FilterCondition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageFilterCondition\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filterCondition\"\n\
  \          },\n          \"description\": \"Contains information about the condition.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-filter-criterion-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CoverageFilterCriterion
---
