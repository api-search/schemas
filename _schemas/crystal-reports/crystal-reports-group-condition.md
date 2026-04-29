---
description: A group condition defining how report data is grouped
layout: schema
name: GroupCondition
properties_list:
- description: Field used for grouping
  name: field
  type: string
- description: Sort direction of the group
  name: direction
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-group-condition-schema.json
slug: crystal-reports-group-condition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-group-condition-schema.json\",\n  \"title\": \"GroupCondition\",\n  \"description\": \"A group condition defining how report data is grouped\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"field\": {\n      \"type\": \"string\",\n      \"description\": \"Field used for grouping\",\n      \"example\": \"Country\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"description\": \"Sort direction of the group\",\n      \"enum\": [\n        \"Ascending\",\n        \"Descending\"\n      ],\n      \"example\": \"Ascending\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-group-condition-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: GroupCondition
---
