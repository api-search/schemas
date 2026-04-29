---
description: <p>The system identified one of the following warnings while processing the input document:</p> <ul> <li> <p>The document to classify is plain text, but the classifier is a native model.</p> </li> <li> <p>The document to classify is semi-structured, but the classifier is a plain-text model.</p> </li> </ul>
layout: schema
name: WarningsListItem
properties_list:
- description: ''
  name: Page
  type: object
- description: ''
  name: WarnCode
  type: object
- description: ''
  name: WarnMessage
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-warnings-list-item-schema.json
slug: openapi.yml-warnings-list-item
source_filename: openapi.yml-warnings-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-warnings-list-item-schema.json\",\n  \"title\": \"WarningsListItem\",\n  \"description\": \"<p>The system identified one of the following warnings while processing the input document:</p> <ul> <li> <p>The document to classify is plain text, but the classifier is a native model.</p> </li> <li> <p>The document to classify is semi-structured, but the classifier is a plain-text model.</p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Page\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Page number in the input document.\"\n        }\n      ]\n    },\n    \"WarnCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageBasedWarningCode\"\n        },\n\
  \        {\n          \"description\": \"The type of warning.\"\n        }\n      ]\n    },\n    \"WarnMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Text message associated with the warning.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-warnings-list-item-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: WarningsListItem
---
