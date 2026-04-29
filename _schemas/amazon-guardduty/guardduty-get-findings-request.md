---
description: GetFindingsRequest schema from Amazon GuardDuty API
layout: schema
name: GetFindingsRequest
properties_list:
- description: ''
  name: FindingIds
  type: object
- description: ''
  name: SortCriteria
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-findings-request-schema.json
slug: guardduty-get-findings-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-findings-request-schema.json\",\n  \"title\": \"GetFindingsRequest\",\n  \"description\": \"GetFindingsRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FindingIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingIds\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"findingIds\"\n          },\n          \"description\": \"The IDs of the findings that you want to retrieve.\"\n        }\n      ]\n    },\n    \"SortCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortCriteria\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sortCriteria\"\n          },\n          \"description\": \"Represents the criteria used for sorting findings.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FindingIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-findings-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetFindingsRequest
---
