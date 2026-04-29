---
description: ''
layout: schema
name: srsExpression
properties_list:
- description: ''
  name: axes
  type: array
- description: ''
  name: names
  type: array
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-srs-expression-schema.json
slug: oneatlas-srs-expression
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-srs-expression-schema.json\",\n  \"title\": \"srsExpression\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"axes\": {\n      \"example\": [\n        {\n          \"abbreviation\": \"Lat\",\n          \"direction\": \"north\"\n        },\n        {\n          \"abbreviation\": \"Lon\",\n          \"direction\": \"east\"\n        }\n      ],\n      \"items\": {\n        \"properties\": {\n          \"abbreviation\": {\n            \"type\": \"string\"\n          },\n          \"direction\": {\n            \"type\": \"string\"\n          }\n        },\n        \"type\": \"object\"\n      },\n      \"type\": \"array\",\n      \"uniqueItems\": true\n    },\n    \"names\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/srs\"\n      },\n      \"type\": \"array\",\n      \"uniqueItems\"\
  : true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-srs-expression-schema.json
tags:
- Imagery
- Satellites
title: srsExpression
---
