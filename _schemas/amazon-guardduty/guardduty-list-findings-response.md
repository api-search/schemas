---
description: ListFindingsResponse schema from Amazon GuardDuty API
layout: schema
name: ListFindingsResponse
properties_list:
- description: ''
  name: FindingIds
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-list-findings-response-schema.json
slug: guardduty-list-findings-response
source_filename: guardduty-list-findings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-findings-response-schema.json\",\n  \"title\": \"ListFindingsResponse\",\n  \"description\": \"ListFindingsResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FindingIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingIds\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"findingIds\"\n          },\n          \"description\": \"The IDs of the findings that you're listing.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"The pagination parameter to be used on the next list operation\
  \ to retrieve more items.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FindingIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-findings-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ListFindingsResponse
---
