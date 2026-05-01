---
description: ListMembersResponse schema from Amazon GuardDuty API
layout: schema
name: ListMembersResponse
properties_list:
- description: ''
  name: Members
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-list-members-response-schema.json
slug: guardduty-list-members-response
source_filename: guardduty-list-members-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-members-response-schema.json\",\n  \"title\": \"ListMembersResponse\",\n  \"description\": \"ListMembersResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Members\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Members\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"members\"\n          },\n          \"description\": \"A list of members.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"The pagination parameter to be used on the next list operation to retrieve more items.\"\n \
  \       }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-members-response-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ListMembersResponse
---
