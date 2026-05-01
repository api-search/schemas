---
description: ListThreatIntelSetsResponse schema from Amazon GuardDuty API
layout: schema
name: ListThreatIntelSetsResponse
properties_list:
- description: ''
  name: ThreatIntelSetIds
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-list-threat-intel-sets-response-schema.json
slug: guardduty-list-threat-intel-sets-response
source_filename: guardduty-list-threat-intel-sets-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-threat-intel-sets-response-schema.json\",\n  \"title\": \"ListThreatIntelSetsResponse\",\n  \"description\": \"ListThreatIntelSetsResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ThreatIntelSetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThreatIntelSetIds\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"threatIntelSetIds\"\n          },\n          \"description\": \"The IDs of the ThreatIntelSet resources.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"The pagination\
  \ parameter to be used on the next list operation to retrieve more items.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ThreatIntelSetIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-threat-intel-sets-response-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ListThreatIntelSetsResponse
---
