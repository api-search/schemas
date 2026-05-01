---
description: Contains information about the criteria used for sorting findings.
layout: schema
name: SortCriteria
properties_list:
- description: ''
  name: AttributeName
  type: object
- description: ''
  name: OrderBy
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-sort-criteria-schema.json
slug: guardduty-sort-criteria
source_filename: guardduty-sort-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-sort-criteria-schema.json\",\n  \"title\": \"SortCriteria\",\n  \"description\": \"Contains information about the criteria used for sorting findings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AttributeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"attributeName\"\n          },\n          \"description\": \"Represents the finding attribute, such as <code>accountId</code>, that sorts the findings.\"\n        }\n      ]\n    },\n    \"OrderBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderBy\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"orderBy\"\n          },\n          \"description\": \"The order by\
  \ which the sorted findings are to be displayed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-sort-criteria-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: SortCriteria
---
