---
description: Information about the sorting criteria used in the coverage statistics.
layout: schema
name: CoverageSortCriteria
properties_list:
- description: ''
  name: AttributeName
  type: object
- description: ''
  name: OrderBy
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-coverage-sort-criteria-schema.json
slug: guardduty-coverage-sort-criteria
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-sort-criteria-schema.json\",\n  \"title\": \"CoverageSortCriteria\",\n  \"description\": \"Information about the sorting criteria used in the coverage statistics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AttributeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageSortKey\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"attributeName\"\n          },\n          \"description\": \"Represents the field name used to sort the coverage details.\"\n        }\n      ]\n    },\n    \"OrderBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderBy\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"orderBy\"\n          },\n          \"description\": \"The order in\
  \ which the sorted findings are to be displayed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-sort-criteria-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CoverageSortCriteria
---
