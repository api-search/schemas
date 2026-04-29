---
description: Paginated list of core facilities.
layout: schema
name: Cores List Response
properties_list:
- description: ''
  name: cores
  type: array
- description: Total number of cores matching the query.
  name: total
  type: integer
- description: Current page number.
  name: page
  type: integer
- description: Number of items per page.
  name: per_page
  type: integer
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-cores-list-response-schema.json
slug: ilab-operations-api-cores-list-response
source_filename: ilab-operations-api-cores-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-cores-list-response-schema.json\",\n  \"title\": \"Cores List Response\",\n  \"description\": \"Paginated list of core facilities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cores\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Core\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of cores matching the query.\",\n      \"example\": 42\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number.\",\n      \"example\": 1\n    },\n    \"per_page\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items per page.\",\n      \"example\": 25\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-cores-list-response-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Cores List Response
---
