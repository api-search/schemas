---
description: A parse job in LlamaParse representing the asynchronous processing of a document through AI-powered parsing with configurable tiers for different quality and speed trade-offs.
layout: schema
name: LlamaIndex Parse Job
properties_list:
- description: Unique identifier of the parse job.
  name: id
  type: string
- description: Current processing status of the parse job.
  name: status
  type: string
- description: Parsing tier that determines quality and speed trade-off. Fast outputs spatial text only. Cost-effective is optimized for text-heavy documents. Agentic handles images and diagrams. Agentic-plus provid
  name: tier
  type: string
- description: API version used for parsing. Use 'latest' for most recent or a specific date string for production stability.
  name: version
  type: string
- description: Identifier of the uploaded file being parsed.
  name: file_id
  type: string
- description: URL of the document fetched for parsing, if provided instead of file_id.
  name: source_url
  type: string
- description: Name of the parsed file.
  name: file_name
  type: string
- description: Total number of pages in the document.
  name: num_pages
  type: integer
- description: Page range to parse using 1-based indexing (e.g., '1-5', '3,7,10').
  name: target_pages
  type: string
- description: ''
  name: result
  type: object
- description: Timestamp when the parse job was created.
  name: created_at
  type: string
- description: Timestamp when the parse job completed.
  name: completed_at
  type: string
provider_name: llamaindex
provider_slug: llamaindex
schema_file: json-schema/llamaindex-parse-job-schema.json
slug: llamaindex-parse-job
source_filename: llamaindex-parse-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://llamaindex.ai/schemas/llamaindex/parse-job.json\",\n  \"title\": \"LlamaIndex Parse Job\",\n  \"description\": \"A parse job in LlamaParse representing the asynchronous processing of a document through AI-powered parsing with configurable tiers for different quality and speed trade-offs.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"status\", \"tier\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the parse job.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"pending\", \"processing\", \"completed\", \"failed\"],\n      \"description\": \"Current processing status of the parse job.\"\n    },\n    \"tier\": {\n      \"type\": \"string\",\n      \"enum\": [\"fast\", \"cost_effective\", \"agentic\", \"agentic_plus\"],\n      \"description\": \"Parsing tier that determines quality and\
  \ speed trade-off. Fast outputs spatial text only. Cost-effective is optimized for text-heavy documents. Agentic handles images and diagrams. Agentic-plus provides maximum fidelity for complex layouts.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"API version used for parsing. Use 'latest' for most recent or a specific date string for production stability.\",\n      \"pattern\": \"^(latest|\\\\d{4}-\\\\d{2}-\\\\d{2})$\"\n    },\n    \"file_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the uploaded file being parsed.\"\n    },\n    \"source_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the document fetched for parsing, if provided instead of file_id.\"\n    },\n    \"file_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the parsed file.\"\n    },\n    \"num_pages\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\"\
  : \"Total number of pages in the document.\"\n    },\n    \"target_pages\": {\n      \"type\": \"string\",\n      \"description\": \"Page range to parse using 1-based indexing (e.g., '1-5', '3,7,10').\",\n      \"pattern\": \"^[\\\\d,\\\\-\\\\s]+$\"\n    },\n    \"result\": {\n      \"$ref\": \"#/$defs/ParseResult\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the parse job was created.\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the parse job completed.\"\n    }\n  },\n  \"$defs\": {\n    \"ParseResult\": {\n      \"type\": \"object\",\n      \"description\": \"The parsed output of a document containing extracted content in various formats.\",\n      \"properties\": {\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"Plain text representation of the parsed content.\"\n\
  \        },\n        \"markdown\": {\n          \"type\": \"string\",\n          \"description\": \"Markdown-formatted representation of the parsed content.\"\n        },\n        \"json\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Structured JSON representation of the parsed content.\"\n        },\n        \"pages\": {\n          \"type\": \"array\",\n          \"description\": \"Per-page parsing results.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/ParsePage\"\n          }\n        },\n        \"metadata\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Metadata extracted from the document.\"\n        }\n      }\n    },\n    \"ParsePage\": {\n      \"type\": \"object\",\n      \"description\": \"Parsed content for a single page of a document.\",\n      \"required\": [\"page_number\"],\n      \"properties\": {\n        \"page_number\": {\n     \
  \     \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"1-based page number.\"\n        },\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"Plain text content of the page.\"\n        },\n        \"markdown\": {\n          \"type\": \"string\",\n          \"description\": \"Markdown-formatted content of the page.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/json-schema/llamaindex-parse-job-schema.json
tags: []
title: LlamaIndex Parse Job
---
