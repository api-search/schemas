---
description: Schema for a Mistral AI OCR response, containing structured page-by-page text extraction results from documents and images.
layout: schema
name: Mistral AI OCR Response
properties_list:
- description: List of pages with extracted OCR content.
  name: pages
  type: array
- description: The model used for OCR processing.
  name: model
  type: string
- description: Usage statistics for the OCR request.
  name: usage
  type: object
provider_name: Mistral AI
provider_slug: mistral-ai
schema_file: json-schema/mistral-ai-ocr-response-schema.json
slug: mistral-ai-ocr-response
source_filename: mistral-ai-ocr-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://mistral.ai/schemas/mistral-ai/ocr-response.json\",\n  \"title\": \"Mistral AI OCR Response\",\n  \"description\": \"Schema for a Mistral AI OCR response, containing structured page-by-page text extraction results from documents and images.\",\n  \"type\": \"object\",\n  \"required\": [\"pages\"],\n  \"$defs\": {\n    \"OcrPage\": {\n      \"type\": \"object\",\n      \"description\": \"A single page of OCR results with extracted markdown content.\",\n      \"required\": [\"index\", \"markdown\"],\n      \"properties\": {\n        \"index\": {\n          \"type\": \"integer\",\n          \"description\": \"The zero-based page index in the document.\",\n          \"minimum\": 0\n        },\n        \"markdown\": {\n          \"type\": \"string\",\n          \"description\": \"Extracted content in markdown format preserving headers, tables, and equations.\"\n        },\n        \"images\"\
  : {\n          \"type\": \"array\",\n          \"description\": \"Extracted images from the page when include_image_base64 was enabled.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/ExtractedImage\"\n          }\n        },\n        \"dimensions\": {\n          \"$ref\": \"#/$defs/PageDimensions\"\n        }\n      }\n    },\n    \"ExtractedImage\": {\n      \"type\": \"object\",\n      \"description\": \"An image extracted from a document page.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the extracted image.\"\n        },\n        \"base64\": {\n          \"type\": \"string\",\n          \"description\": \"Base64-encoded image data.\"\n        },\n        \"content_type\": {\n          \"type\": \"string\",\n          \"description\": \"MIME type of the image.\",\n          \"pattern\": \"^image/[a-z]+$\"\n        }\n      }\n    },\n    \"PageDimensions\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"The dimensions of a document page.\",\n      \"properties\": {\n        \"width\": {\n          \"type\": \"integer\",\n          \"description\": \"Page width in pixels.\",\n          \"minimum\": 1\n        },\n        \"height\": {\n          \"type\": \"integer\",\n          \"description\": \"Page height in pixels.\",\n          \"minimum\": 1\n        }\n      }\n    }\n  },\n  \"properties\": {\n    \"pages\": {\n      \"type\": \"array\",\n      \"description\": \"List of pages with extracted OCR content.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/OcrPage\"\n      }\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model used for OCR processing.\"\n    },\n    \"usage\": {\n      \"type\": \"object\",\n      \"description\": \"Usage statistics for the OCR request.\",\n      \"properties\": {\n        \"pages_processed\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of pages processed.\"\
  ,\n          \"minimum\": 0\n        },\n        \"doc_size_bytes\": {\n          \"type\": \"integer\",\n          \"description\": \"Document size in bytes.\",\n          \"minimum\": 0\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/json-schema/mistral-ai-ocr-response-schema.json
tags:
- Agents
- Artificial Intelligence
- Batch Processing
- Chat
- Embeddings
- Fine-Tuning
- Large Language Models
- OCR
title: Mistral AI OCR Response
---
