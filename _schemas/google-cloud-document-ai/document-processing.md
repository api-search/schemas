---
description: Schema for a Google Cloud Document AI processing request.
layout: schema
name: Document Processing Request
properties_list:
- description: An inline document for processing.
  name: inlineDocument
  type: object
- description: A raw document provided as bytes.
  name: rawDocument
  type: object
- description: Whether to skip the human review stage.
  name: skipHumanReview
  type: boolean
- description: Specifies which fields to include in the output document.
  name: fieldMask
  type: string
provider_name: Google Cloud Document AI
provider_slug: google-cloud-document-ai
schema_file: json-schema/document-processing.json
slug: document-processing
source_filename: document-processing.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-document-ai/refs/heads/main/json-schema/document-processing.json\",\n  \"title\": \"Document Processing Request\",\n  \"description\": \"Schema for a Google Cloud Document AI processing request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inlineDocument\": {\n      \"type\": \"object\",\n      \"description\": \"An inline document for processing.\",\n      \"properties\": {\n        \"mimeType\": {\n          \"type\": \"string\",\n          \"description\": \"MIME type of the document.\"\n        },\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"UTF-8 encoded text of the document.\"\n        },\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"Base64-encoded document content.\"\n        }\n      }\n    },\n    \"rawDocument\": {\n      \"type\": \"\
  object\",\n      \"description\": \"A raw document provided as bytes.\",\n      \"properties\": {\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"Base64-encoded document content.\"\n        },\n        \"mimeType\": {\n          \"type\": \"string\",\n          \"description\": \"MIME type of the raw document.\"\n        }\n      }\n    },\n    \"skipHumanReview\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to skip the human review stage.\"\n    },\n    \"fieldMask\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies which fields to include in the output document.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-document-ai/refs/heads/main/json-schema/document-processing.json
tags:
- Data Extraction
- Document Processing
- Forms
- Google Cloud
- Machine Learning
- OCR
title: Document Processing Request
---
