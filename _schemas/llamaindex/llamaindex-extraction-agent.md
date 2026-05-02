---
description: An extraction agent in LlamaExtract configured with a specific data schema and extraction settings for transforming unstructured documents into structured JSON representations.
layout: schema
name: LlamaIndex Extraction Agent
properties_list:
- description: Unique identifier of the extraction agent.
  name: id
  type: string
- description: Human-readable name of the extraction agent.
  name: name
  type: string
- description: Identifier of the project the agent belongs to.
  name: project_id
  type: string
- description: Optional description of the extraction agent and its purpose.
  name: description
  type: string
- description: JSON Schema defining the structure of the data to extract from documents.
  name: data_schema
  type: object
- description: Optional prompt used for automatic schema inference from example documents.
  name: prompt
  type: string
- description: Extraction jobs that have been run with this agent.
  name: extraction_jobs
  type: array
- description: Timestamp when the extraction agent was created.
  name: created_at
  type: string
- description: Timestamp when the extraction agent was last updated.
  name: updated_at
  type: string
provider_name: llamaindex
provider_slug: llamaindex
schema_file: json-schema/llamaindex-extraction-agent-schema.json
slug: llamaindex-extraction-agent
source_filename: llamaindex-extraction-agent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://llamaindex.ai/schemas/llamaindex/extraction-agent.json\",\n  \"title\": \"LlamaIndex Extraction Agent\",\n  \"description\": \"An extraction agent in LlamaExtract configured with a specific data schema and extraction settings for transforming unstructured documents into structured JSON representations.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"project_id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the extraction agent.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the extraction agent.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the project the agent belongs to.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Optional description of the extraction agent and its purpose.\",\n      \"maxLength\": 1000\n    },\n    \"data_schema\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"JSON Schema defining the structure of the data to extract from documents.\"\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Optional prompt used for automatic schema inference from example documents.\"\n    },\n    \"extraction_jobs\": {\n      \"type\": \"array\",\n      \"description\": \"Extraction jobs that have been run with this agent.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ExtractionJob\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the extraction agent was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp\
  \ when the extraction agent was last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"ExtractionJob\": {\n      \"type\": \"object\",\n      \"description\": \"An asynchronous extraction job that processes documents through an extraction agent.\",\n      \"required\": [\"id\", \"extraction_agent_id\", \"status\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the extraction job.\"\n        },\n        \"extraction_agent_id\": {\n          \"type\": \"string\",\n          \"description\": \"Identifier of the extraction agent used for this job.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"pending\", \"processing\", \"completed\", \"failed\"],\n          \"description\": \"Current status of the extraction job.\"\n        },\n        \"file_ids\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n         \
  \ \"description\": \"Identifiers of the files being processed.\"\n        },\n        \"results\": {\n          \"type\": \"array\",\n          \"description\": \"Extraction results for each processed file.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/FileExtractionResult\"\n          }\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the extraction job was created.\"\n        },\n        \"completed_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the extraction job completed.\"\n        }\n      }\n    },\n    \"FileExtractionResult\": {\n      \"type\": \"object\",\n      \"description\": \"Extraction result for a single processed file.\",\n      \"required\": [\"file_id\", \"status\"],\n      \"properties\": {\n        \"file_id\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Identifier of the processed file.\"\n        },\n        \"file_name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the processed file.\"\n        },\n        \"data\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Structured data extracted from the file, conforming to the agent data schema.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"success\", \"error\"],\n          \"description\": \"Extraction status for this specific file.\"\n        },\n        \"error\": {\n          \"type\": \"string\",\n          \"description\": \"Error message if extraction failed for this file.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/llamaindex/refs/heads/main/json-schema/llamaindex-extraction-agent-schema.json
tags: []
title: LlamaIndex Extraction Agent
---
