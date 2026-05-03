---
description: Represents a dataset used for training Einstein Vision or Language models, including labels, examples, and metadata.
layout: schema
name: Einstein Dataset
properties_list:
- description: Unique dataset identifier.
  name: id
  type: integer
- description: Name of the dataset.
  name: name
  type: string
- description: Type of the dataset.
  name: type
  type: string
- description: Timestamp when the dataset was created.
  name: createdAt
  type: string
- description: Timestamp when the dataset was last updated.
  name: updatedAt
  type: string
- description: Total number of examples in the dataset.
  name: totalExamples
  type: integer
- description: Total number of labels in the dataset.
  name: totalLabels
  type: integer
- description: Whether the dataset is available for training and predictions.
  name: available
  type: boolean
- description: Status message describing the dataset's current state.
  name: statusMsg
  type: string
- description: Summary of labels in the dataset.
  name: labelSummary
  type: object
- description: Object type identifier.
  name: object
  type: string
provider_name: Salesforce Einstein
provider_slug: salesforce-einstein
schema_file: json-schema/salesforce-einstein-dataset-schema.json
slug: salesforce-einstein-dataset
source_filename: salesforce-einstein-dataset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/salesforce-einstein/json-schema/salesforce-einstein-dataset-schema.json\",\n  \"title\": \"Einstein Dataset\",\n  \"description\": \"Represents a dataset used for training Einstein Vision or Language models, including labels, examples, and metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique dataset identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the dataset.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the dataset.\",\n      \"enum\": [\n        \"image\",\n        \"image-multi-label\",\n        \"image-detection\",\n        \"text-sentiment\",\n        \"text-intent\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Timestamp when the dataset was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the dataset was last updated.\"\n    },\n    \"totalExamples\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of examples in the dataset.\",\n      \"minimum\": 0\n    },\n    \"totalLabels\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of labels in the dataset.\",\n      \"minimum\": 0\n    },\n    \"available\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the dataset is available for training and predictions.\"\n    },\n    \"statusMsg\": {\n      \"type\": \"string\",\n      \"description\": \"Status message describing the dataset's current state.\"\n    },\n    \"labelSummary\": {\n      \"type\": \"object\",\n      \"description\": \"Summary of labels in the dataset.\",\n      \"properties\": {\n        \"labels\": {\n          \"\
  type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Label\"\n          }\n        }\n      }\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"Object type identifier.\",\n      \"const\": \"dataset\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"type\"],\n  \"$defs\": {\n    \"Label\": {\n      \"type\": \"object\",\n      \"description\": \"A label within a dataset used to classify examples.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique label identifier.\"\n        },\n        \"datasetId\": {\n          \"type\": \"integer\",\n          \"description\": \"ID of the dataset this label belongs to.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the label.\"\n        },\n        \"numExamples\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of examples with this label.\",\n\
  \          \"minimum\": 0\n        }\n      },\n      \"required\": [\"id\", \"name\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/json-schema/salesforce-einstein-dataset-schema.json
tags:
- Artificial Intelligence
- Computer Vision
- CRM
- Machine Learning
- Natural Language Processing
- Predictive Analytics
- Salesforce
title: Einstein Dataset
---
