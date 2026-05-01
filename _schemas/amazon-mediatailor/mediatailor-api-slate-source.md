---
description: Slate VOD source configuration.
layout: schema
name: SlateSource
properties_list:
- description: ''
  name: SourceLocationName
  type: object
- description: ''
  name: VodSourceName
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-slate-source-schema.json
slug: mediatailor-api-slate-source
source_filename: mediatailor-api-slate-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-slate-source-schema.json\",\n  \"title\": \"SlateSource\",\n  \"description\": \"Slate VOD source configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceLocationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the source location where the slate VOD source is stored.\"\n        }\n      ]\n    },\n    \"VodSourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The slate VOD source name. The VOD source must already exist in a source location before it can be used for slate.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-slate-source-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: SlateSource
---
