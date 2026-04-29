---
description: ''
layout: schema
name: search-options-v2
properties_list: []
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-search-options-v2-schema.json
slug: oneatlas-search-options-v2
source_filename: oneatlas-search-options-v2-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-search-options-v2-schema.json\",\n  \"title\": \"search-options-v2\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/search-options\"\n    },\n    {\n      \"properties\": {\n        \"acquisitionIdentifier\": {\n          \"type\": \"string\",\n          \"description\": \"The acquisition identifier\",\n          \"example\": \"DS_PNEO3_201602011017034\"\n        },\n        \"archiveAnonymousIdentifier\": {\n          \"type\": \"string\",\n          \"description\": \"The archive anonymous identifier\",\n          \"example\": \"31476131\"\n        },\n        \"archiveIdentifier\": {\n          \"type\": \"string\",\n          \"description\": \"The archive identifier\",\n          \"example\": \"DS_SPOT7_201412071054567_FR1_FR1_FR1_FR1_W003N39_01709\"\n        }\n      }\n\
  \    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-search-options-v2-schema.json
tags:
- Imagery
- Satellites
title: search-options-v2
---
