---
description: Describes information about a document classifier and its versions.
layout: schema
name: DocumentClassifierSummary
properties_list:
- description: ''
  name: DocumentClassifierName
  type: object
- description: ''
  name: NumberOfVersions
  type: object
- description: ''
  name: LatestVersionCreatedAt
  type: object
- description: ''
  name: LatestVersionName
  type: object
- description: ''
  name: LatestVersionStatus
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-document-classifier-summary-schema.json
slug: openapi.yml-document-classifier-summary
source_filename: openapi.yml-document-classifier-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-classifier-summary-schema.json\",\n  \"title\": \"DocumentClassifierSummary\",\n  \"description\": \"Describes information about a document classifier and its versions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocumentClassifierName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArnName\"\n        },\n        {\n          \"description\": \"The name that you assigned the document classifier.\"\n        }\n      ]\n    },\n    \"NumberOfVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of versions you created.\"\n        }\n      ]\n    },\n    \"LatestVersionCreatedAt\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that the latest document classifier version was submitted for processing.\"\n        }\n      ]\n    },\n    \"LatestVersionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionName\"\n        },\n        {\n          \"description\": \"The version name you assigned to the latest document classifier version.\"\n        }\n      ]\n    },\n    \"LatestVersionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelStatus\"\n        },\n        {\n          \"description\": \"Provides the status of the latest document classifier version.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-classifier-summary-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DocumentClassifierSummary
---
