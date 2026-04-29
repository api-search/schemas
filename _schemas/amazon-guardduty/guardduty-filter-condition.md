---
description: Contains information about the condition.
layout: schema
name: FilterCondition
properties_list:
- description: ''
  name: EqualsValue
  type: object
- description: ''
  name: GreaterThan
  type: object
- description: ''
  name: LessThan
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-filter-condition-schema.json
slug: guardduty-filter-condition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-filter-condition-schema.json\",\n  \"title\": \"FilterCondition\",\n  \"description\": \"Contains information about the condition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EqualsValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"equalsValue\"\n          },\n          \"description\": \"Represents an <i>equal</i> <b/> condition to be applied to a single field when querying for scan entries.\"\n        }\n      ]\n    },\n    \"GreaterThan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongValue\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"greaterThan\"\n          },\n          \"description\": \"Represents\
  \ a <i>greater than</i> condition to be applied to a single field when querying for scan entries.\"\n        }\n      ]\n    },\n    \"LessThan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongValue\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lessThan\"\n          },\n          \"description\": \"Represents a <i>less than</i> condition to be applied to a single field when querying for scan entries.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-filter-condition-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: FilterCondition
---
