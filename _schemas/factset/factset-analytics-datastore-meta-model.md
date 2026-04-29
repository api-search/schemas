---
description: Meta model which includes pagination information
layout: schema
name: MetaModel
properties_list:
- description: Pagination attributes for the offset-based pagination strategy
  name: pagination
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-analytics-datastore-meta-model-schema.json
slug: factset-analytics-datastore-meta-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetaModel\",\n  \"type\": \"object\",\n  \"description\": \"Meta model which includes pagination information\",\n  \"properties\": {\n    \"pagination\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination attributes for the offset-based pagination strategy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-analytics-datastore-meta-model-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: MetaModel
---
