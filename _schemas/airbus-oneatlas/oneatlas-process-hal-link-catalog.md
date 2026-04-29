---
description: ''
layout: schema
name: processHALLinkCatalog
properties_list: []
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-process-hal-link-catalog-schema.json
slug: oneatlas-process-hal-link-catalog
source_filename: oneatlas-process-hal-link-catalog-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-process-hal-link-catalog-schema.json\",\n  \"title\": \"processHALLinkCatalog\",\n  \"allOf\": [\n    {\n      \"properties\": {\n        \"description\": {\n          \"allOf\": [\n            {\n              \"description\": \"See [Describe process](#/paths/~1api~1v1~1processes~1{processId}/post)\"\n            },\n            {\n              \"$ref\": \"#/components/schemas/Link\"\n            }\n          ]\n        }\n      },\n      \"type\": \"object\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/processHALLinkCommon\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-process-hal-link-catalog-schema.json
tags:
- Imagery
- Satellites
title: processHALLinkCatalog
---
