---
description: Basic LookML model information
layout: schema
name: LookModel
properties_list:
- description: Model name/identifier
  name: id
  type: string
- description: Display label for the model
  name: label
  type: string
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-look-model-schema.json
slug: looker-look-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LookModel\",\n  \"type\": \"object\",\n  \"description\": \"Basic LookML model information\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Model name/identifier\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Display label for the model\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-look-model-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: LookModel
---
