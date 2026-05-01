---
description: Splice insert message configuration.
layout: schema
name: SpliceInsertMessage
properties_list:
- description: ''
  name: AvailNum
  type: object
- description: ''
  name: AvailsExpected
  type: object
- description: ''
  name: SpliceEventId
  type: object
- description: ''
  name: UniqueProgramId
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-splice-insert-message-schema.json
slug: mediatailor-api-splice-insert-message
source_filename: mediatailor-api-splice-insert-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-splice-insert-message-schema.json\",\n  \"title\": \"SpliceInsertMessage\",\n  \"description\": \"Splice insert message configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailNum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"This is written to <code>splice_insert.avail_num</code>, as defined in section 9.7.3.1 of the SCTE-35 specification. The default value is <code>0</code>. Values must be between <code>0</code> and <code>256</code>, inclusive.\"\n        }\n      ]\n    },\n    \"AvailsExpected\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"This is written to <code>splice_insert.avails_expected</code>,\
  \ as defined in section 9.7.3.1 of the SCTE-35 specification. The default value is <code>0</code>. Values must be between <code>0</code> and <code>256</code>, inclusive.\"\n        }\n      ]\n    },\n    \"SpliceEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"This is written to <code>splice_insert.splice_event_id</code>, as defined in section 9.7.3.1 of the SCTE-35 specification. The default value is <code>1</code>.\"\n        }\n      ]\n    },\n    \"UniqueProgramId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"This is written to <code>splice_insert.unique_program_id</code>, as defined in section 9.7.3.1 of the SCTE-35 specification. The default value is <code>0</code>. Values must be between <code>0</code> and <code>256</code>, inclusive.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-splice-insert-message-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: SpliceInsertMessage
---
