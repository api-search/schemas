---
description: ListFiltersResponse schema from Amazon GuardDuty API
layout: schema
name: ListFiltersResponse
properties_list:
- description: ''
  name: FilterNames
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-list-filters-response-schema.json
slug: guardduty-list-filters-response
source_filename: guardduty-list-filters-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-filters-response-schema.json\",\n  \"title\": \"ListFiltersResponse\",\n  \"description\": \"ListFiltersResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FilterNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterNames\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filterNames\"\n          },\n          \"description\": \"A list of filter names.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"The pagination parameter to be used on the next list operation to retrieve\
  \ more items.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FilterNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-filters-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ListFiltersResponse
---
