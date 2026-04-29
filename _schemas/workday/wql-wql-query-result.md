---
description: ''
layout: schema
name: WqlQueryResult
properties_list:
- description: The array of result rows from the WQL query.
  name: data
  type: array
- description: The total number of results available.
  name: total
  type: integer
provider_name: Workday
provider_slug: workday
schema_file: json-schema/wql-wql-query-result-schema.json
slug: wql-wql-query-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WqlQueryResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"The array of result rows from the WQL query.\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of results available.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/wql-wql-query-result-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: WqlQueryResult
---
