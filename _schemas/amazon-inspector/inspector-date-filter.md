---
description: Contains details on the time range used to filter findings.
layout: schema
name: DateFilter
properties_list:
- description: ''
  name: endInclusive
  type: object
- description: ''
  name: startInclusive
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-date-filter-schema.json
slug: inspector-date-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-date-filter-schema.json\",\n  \"title\": \"DateFilter\",\n  \"description\": \"Contains details on the time range used to filter findings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endInclusive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp representing the end of the time period filtered on.\"\n        }\n      ]\n    },\n    \"startInclusive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp representing the start of the time period filtered on.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-date-filter-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: DateFilter
---
