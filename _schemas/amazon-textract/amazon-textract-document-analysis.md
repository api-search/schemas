---
description: Response object containing the results of document text detection or analysis, including detected blocks of text, tables, and forms.
layout: schema
name: DocumentAnalysis
properties_list:
- description: Metadata about the document.
  name: DocumentMetadata
  type: object
- description: The items detected in the document.
  name: Blocks
  type: array
- description: The version of the model used to analyze the document.
  name: AnalyzeDocumentModelVersion
  type: string
provider_name: Amazon Textract
provider_slug: amazon-textract
schema_file: json-schema/amazon-textract-document-analysis-schema.json
slug: amazon-textract-document-analysis
source_filename: amazon-textract-document-analysis-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response object containing the results of document text detection or analysis, including detected blocks of text, tables, and forms.\",\n  \"properties\": {\n    \"DocumentMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about the document.\",\n      \"properties\": {\n        \"Pages\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of pages detected in the document.\"\n        }\n      }\n    },\n    \"Blocks\": {\n      \"type\": \"array\",\n      \"description\": \"The items detected in the document.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"BlockType\": {\n            \"type\": \"string\",\n            \"description\": \"The type of text item detected.\",\n            \"enum\": [\n              \"KEY_VALUE_SET\",\n              \"PAGE\",\n              \"LINE\",\n              \"WORD\",\n              \"TABLE\"\
  ,\n              \"CELL\",\n              \"SELECTION_ELEMENT\",\n              \"MERGED_CELL\",\n              \"TITLE\",\n              \"QUERY\",\n              \"QUERY_RESULT\",\n              \"SIGNATURE\",\n              \"TABLE_TITLE\",\n              \"TABLE_FOOTER\",\n              \"LAYOUT_TEXT\",\n              \"LAYOUT_TITLE\",\n              \"LAYOUT_HEADER\",\n              \"LAYOUT_FOOTER\",\n              \"LAYOUT_SECTION_HEADER\",\n              \"LAYOUT_PAGE_NUMBER\",\n              \"LAYOUT_LIST\",\n              \"LAYOUT_FIGURE\",\n              \"LAYOUT_TABLE\",\n              \"LAYOUT_KEY_VALUE\"\n            ]\n          },\n          \"Confidence\": {\n            \"type\": \"number\",\n            \"format\": \"float\",\n            \"description\": \"The confidence score for the detected block.\"\n          },\n          \"Text\": {\n            \"type\": \"string\",\n            \"description\": \"The word or line of text recognized.\"\n          },\n       \
  \   \"Geometry\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"BoundingBox\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"Width\": {\n                    \"type\": \"number\"\n                  },\n                  \"Height\": {\n                    \"type\": \"number\"\n                  },\n                  \"Left\": {\n                    \"type\": \"number\"\n                  },\n                  \"Top\": {\n                    \"type\": \"number\"\n                  }\n                }\n              },\n              \"Polygon\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"X\": {\n                      \"type\": \"number\"\n                    },\n                    \"Y\": {\n                      \"type\": \"number\"\n                    }\n               \
  \   }\n                }\n              }\n            }\n          },\n          \"Id\": {\n            \"type\": \"string\",\n            \"description\": \"The identifier for the recognized text block.\"\n          },\n          \"Relationships\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Type\": {\n                  \"type\": \"string\",\n                  \"enum\": [\n                    \"VALUE\",\n                    \"CHILD\",\n                    \"COMPLEX_FEATURES\",\n                    \"MERGED_CELL\",\n                    \"TITLE\",\n                    \"ANSWER\",\n                    \"TABLE\",\n                    \"TABLE_TITLE\",\n                    \"TABLE_FOOTER\"\n                  ]\n                },\n                \"Ids\": {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"string\"\n             \
  \     }\n                }\n              }\n            }\n          },\n          \"Page\": {\n            \"type\": \"integer\",\n            \"description\": \"The page on which the block was detected.\"\n          }\n        }\n      }\n    },\n    \"AnalyzeDocumentModelVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the model used to analyze the document.\"\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DocumentAnalysis\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-textract/refs/heads/main/json-schema/amazon-textract-document-analysis-schema.json
tags:
- Document Processing
- Machine Learning
- OCR
title: DocumentAnalysis
---
