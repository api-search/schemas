---
description: List of available datasets in the Data Cloud
layout: schema
name: DatasetList
properties_list:
- description: ''
  name: datasets
  type: array
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-data-cloud-dataset-list-schema.json
slug: aladdin-studio-data-cloud-dataset-list
source_filename: aladdin-studio-data-cloud-dataset-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-data-cloud-dataset-list-schema.json\",\n  \"title\": \"DatasetList\",\n  \"description\": \"List of available datasets in the Data Cloud\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"datasets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Dataset\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-data-cloud-dataset-list-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: DatasetList
---
