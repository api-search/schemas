---
description: A dataset produced from a campaign containing downloadable resources.
layout: schema
name: Dataset
properties_list:
- description: Dataset identifier.
  name: datasetId
  type: string
- description: Parent campaign identifier.
  name: campaignId
  type: string
- description: Dataset status.
  name: status
  type: string
- description: ''
  name: resources
  type: array
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-dataset-schema.json
slug: arlula-dataset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/dataset.json\",\n  \"title\": \"Dataset\",\n  \"description\": \"A dataset produced from a campaign containing downloadable resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"datasetId\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset identifier.\",\n      \"examples\": [\n        \"dataset-a1b2c3d4\"\n      ]\n    },\n    \"campaignId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent campaign identifier.\",\n      \"examples\": [\n        \"campaign-a1b2\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset status.\",\n      \"examples\": [\n        \"completed\"\n      ]\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"https://arlula.com/json-schema/resource.json\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-dataset-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: Dataset
---
