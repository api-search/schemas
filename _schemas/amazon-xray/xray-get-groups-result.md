---
description: GetGroupsResult schema from Amazon X-Ray API
layout: schema
name: GetGroupsResult
properties_list:
- description: ''
  name: Groups
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-groups-result-schema.json
slug: xray-get-groups-result
source_filename: xray-get-groups-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Groups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupSummaryList\"\n        },\n        {\n          \"description\": \"The collection of all active groups.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetGroupsResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-groups-result-schema.json\",\n  \"description\": \"GetGroupsResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-groups-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetGroupsResult
---
