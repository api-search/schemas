---
description: ''
layout: schema
name: processHALCatalog
properties_list: []
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-process-hal-catalog-schema.json
slug: oneatlas-process-hal-catalog
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-process-hal-catalog-schema.json\",\n  \"title\": \"processHALCatalog\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/process\"\n    },\n    {\n      \"properties\": {\n        \"_links\": {\n          \"$ref\": \"#/components/schemas/processHALLinkCatalog\"\n        }\n      },\n      \"type\": \"object\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-process-hal-catalog-schema.json
tags:
- Imagery
- Satellites
title: processHALCatalog
---
