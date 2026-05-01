---
description: Schema for a Google Cloud Natural Language document analysis request.
layout: schema
name: Document Analysis
properties_list:
- description: The document to analyze.
  name: document
  type: object
- description: The features to enable for analysis.
  name: features
  type: object
- description: The encoding type for calculating offsets.
  name: encodingType
  type: string
provider_name: Google Cloud Natural Language
provider_slug: google-cloud-natural-language
schema_file: json-schema/document-analysis.json
slug: document-analysis
source_filename: document-analysis.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-natural-language/refs/heads/main/json-schema/document-analysis.json\",\n  \"title\": \"Document Analysis\",\n  \"description\": \"Schema for a Google Cloud Natural Language document analysis request.\",\n  \"type\": \"object\",\n  \"required\": [\"document\"],\n  \"properties\": {\n    \"document\": {\n      \"type\": \"object\",\n      \"description\": \"The document to analyze.\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"TYPE_UNSPECIFIED\", \"PLAIN_TEXT\", \"HTML\"],\n          \"description\": \"The type of the document.\"\n        },\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"The content of the document as a string.\"\n        },\n        \"gcsContentUri\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"Google Cloud Storage URI for the document content.\"\n        },\n        \"language\": {\n          \"type\": \"string\",\n          \"description\": \"BCP-47 language code of the document.\"\n        }\n      }\n    },\n    \"features\": {\n      \"type\": \"object\",\n      \"description\": \"The features to enable for analysis.\",\n      \"properties\": {\n        \"extractSyntax\": {\n          \"type\": \"boolean\",\n          \"description\": \"Extract syntax information.\"\n        },\n        \"extractEntities\": {\n          \"type\": \"boolean\",\n          \"description\": \"Extract entities.\"\n        },\n        \"extractDocumentSentiment\": {\n          \"type\": \"boolean\",\n          \"description\": \"Extract document-level sentiment.\"\n        },\n        \"extractEntitySentiment\": {\n          \"type\": \"boolean\",\n          \"description\": \"Extract entity-level sentiment.\"\n        },\n        \"classifyText\": {\n          \"\
  type\": \"boolean\",\n          \"description\": \"Classify the document into categories.\"\n        }\n      }\n    },\n    \"encodingType\": {\n      \"type\": \"string\",\n      \"enum\": [\"NONE\", \"UTF8\", \"UTF16\", \"UTF32\"],\n      \"description\": \"The encoding type for calculating offsets.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-natural-language/refs/heads/main/json-schema/document-analysis.json
tags:
- Entity Recognition
- Google Cloud
- Machine Learning
- Natural Language Processing
- Sentiment Analysis
- Text Analysis
title: Document Analysis
---
