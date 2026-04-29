---
description: ''
layout: schema
name: JSONLDGraph
properties_list:
- description: ''
  name: '@context'
  type: array
- description: ''
  name: '@graph'
  type: array
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-weather-service-jsonldgraph-schema.json
slug: agstack-openagri-weather-service-jsonldgraph
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/JSONLDGraph.json\",\n  \"title\": \"JSONLDGraph\",\n  \"properties\": {\n    \"@context\": {\n      \"items\": {\n        \"anyOf\": [\n          {\n            \"type\": \"string\"\n          },\n          {\n            \"type\": \"object\"\n          }\n        ]\n      },\n      \"type\": \"array\",\n      \"title\": \"@Context\"\n    },\n    \"@graph\": {\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"type\": \"array\",\n      \"title\": \"@Graph\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"@context\",\n    \"@graph\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-weather-service-jsonldgraph-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: JSONLDGraph
---
