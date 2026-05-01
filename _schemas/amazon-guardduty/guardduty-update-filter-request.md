---
description: UpdateFilterRequest schema from Amazon GuardDuty API
layout: schema
name: UpdateFilterRequest
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: Action
  type: object
- description: ''
  name: Rank
  type: object
- description: ''
  name: FindingCriteria
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-update-filter-request-schema.json
slug: guardduty-update-filter-request
source_filename: guardduty-update-filter-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-update-filter-request-schema.json\",\n  \"title\": \"UpdateFilterRequest\",\n  \"description\": \"UpdateFilterRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterDescription\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"The description of the filter. Valid characters include alphanumeric characters, and special characters such as hyphen, period, colon, underscore, parentheses (<code>{ }</code>, <code>[ ]</code>, and <code>( )</code>), forward slash, horizontal tab, vertical tab, newline, form feed, return, and whitespace.\"\n        }\n      ]\n    },\n    \"Action\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterAction\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"action\"\n          },\n          \"description\": \"Specifies the action that is to be applied to the findings that match the filter.\"\n        }\n      ]\n    },\n    \"Rank\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterRank\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rank\"\n          },\n          \"description\": \"Specifies the position of the filter in the list of current filters. Also specifies the order in which this filter is applied to the findings.\"\n        }\n      ]\n    },\n    \"FindingCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingCriteria\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"findingCriteria\"\n          },\n          \"description\": \"Represents the criteria\
  \ to be used in the filter for querying findings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-update-filter-request-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UpdateFilterRequest
---
