---
description: Paginated list of datasets.
layout: schema
name: DatasetsListResponse
properties_list:
- description: ''
  name: datasets
  type: array
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-datasets-list-response-schema.json
slug: arlula-datasets-list-response
source_filename: arlula-datasets-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/datasets-list-response.json\",\n  \"title\": \"DatasetsListResponse\",\n  \"description\": \"Paginated list of datasets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"datasets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"https://arlula.com/json-schema/dataset.json\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-datasets-list-response-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: DatasetsListResponse
---
