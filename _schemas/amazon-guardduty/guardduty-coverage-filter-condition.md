---
description: Represents a condition that when matched will be added to the response of the operation.
layout: schema
name: CoverageFilterCondition
properties_list:
- description: ''
  name: Equals
  type: object
- description: ''
  name: NotEquals
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-coverage-filter-condition-schema.json
slug: guardduty-coverage-filter-condition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-filter-condition-schema.json\",\n  \"title\": \"CoverageFilterCondition\",\n  \"description\": \"Represents a condition that when matched will be added to the response of the operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Equals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Equals\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"equals\"\n          },\n          \"description\": \"Represents an equal condition that is applied to a single field while retrieving the coverage details.\"\n        }\n      ]\n    },\n    \"NotEquals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotEquals\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"notEquals\"\n      \
  \    },\n          \"description\": \"Represents a not equal condition that is applied to a single field while retrieving the coverage details.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-filter-condition-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CoverageFilterCondition
---
