---
description: Fec Output Settings
layout: schema
name: FecOutputSettings
properties_list:
- description: ''
  name: ColumnDepth
  type: object
- description: ''
  name: IncludeFec
  type: object
- description: ''
  name: RowLength
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-fec-output-settings-schema.json
slug: medialive-api-fec-output-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-fec-output-settings-schema.json\",\n  \"title\": \"FecOutputSettings\",\n  \"description\": \"Fec Output Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ColumnDepth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin4Max20\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"columnDepth\"\n          },\n          \"description\": \"Parameter D from SMPTE 2022-1. The height of the FEC protection matrix.  The number of transport stream packets per column error correction packet. Must be between 4 and 20, inclusive.\"\n        }\n      ]\n    },\n    \"IncludeFec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FecOutputIncludeFec\"\n        },\n        {\n          \"xml\": {\n     \
  \       \"name\": \"includeFec\"\n          },\n          \"description\": \"Enables column only or column and row based FEC\"\n        }\n      ]\n    },\n    \"RowLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max20\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rowLength\"\n          },\n          \"description\": \"Parameter L from SMPTE 2022-1. The width of the FEC protection matrix.  Must be between 1 and 20, inclusive. If only Column FEC is used, then larger values increase robustness.  If Row FEC is used, then this is the number of transport stream packets per row error correction packet, and the value must be between 4 and 20, inclusive, if includeFec is columnAndRow. If includeFec is column, this value must be 1 to 20, inclusive.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-fec-output-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: FecOutputSettings
---
