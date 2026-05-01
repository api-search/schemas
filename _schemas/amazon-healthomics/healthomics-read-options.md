---
description: Read options for an annotation import job.
layout: schema
name: ReadOptions
properties_list:
- description: ''
  name: sep
  type: object
- description: ''
  name: encoding
  type: object
- description: ''
  name: quote
  type: object
- description: ''
  name: quoteAll
  type: object
- description: ''
  name: escape
  type: object
- description: ''
  name: escapeQuotes
  type: object
- description: ''
  name: comment
  type: object
- description: ''
  name: header
  type: object
- description: ''
  name: lineSep
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-read-options-schema.json
slug: healthomics-read-options
source_filename: healthomics-read-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-read-options-schema.json\",\n  \"title\": \"ReadOptions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sep\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Separator\"\n        },\n        {\n          \"description\": \"The file's field separator.\"\n        }\n      ]\n    },\n    \"encoding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Encoding\"\n        },\n        {\n          \"description\": \"The file's encoding.\"\n        }\n      ]\n    },\n    \"quote\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Quote\"\n        },\n        {\n          \"description\": \"The file's quote character.\"\n        }\n      ]\n    },\n    \"quoteAll\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/QuoteAll\"\n        },\n        {\n          \"description\": \"Whether all values need to be quoted, or just those that contain quotes.\"\n        }\n      ]\n    },\n    \"escape\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EscapeChar\"\n        },\n        {\n          \"description\": \"A character for escaping quotes in the file.\"\n        }\n      ]\n    },\n    \"escapeQuotes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EscapeQuotes\"\n        },\n        {\n          \"description\": \"Whether quotes need to be escaped in the file.\"\n        }\n      ]\n    },\n    \"comment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CommentChar\"\n        },\n        {\n          \"description\": \"The file's comment character.\"\n        }\n      ]\n    },\n    \"header\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Header\"\
  \n        },\n        {\n          \"description\": \"Whether the file has a header row.\"\n        }\n      ]\n    },\n    \"lineSep\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LineSep\"\n        },\n        {\n          \"description\": \"A line separator for the file.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Read options for an annotation import job.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-read-options-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ReadOptions
---
