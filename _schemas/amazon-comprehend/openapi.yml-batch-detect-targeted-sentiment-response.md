---
description: BatchDetectTargetedSentimentResponse schema
layout: schema
name: BatchDetectTargetedSentimentResponse
properties_list:
- description: ''
  name: ResultList
  type: object
- description: ''
  name: ErrorList
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-batch-detect-targeted-sentiment-response-schema.json
slug: openapi.yml-batch-detect-targeted-sentiment-response
source_filename: openapi.yml-batch-detect-targeted-sentiment-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-batch-detect-targeted-sentiment-response-schema.json\",\n  \"title\": \"BatchDetectTargetedSentimentResponse\",\n  \"description\": \"BatchDetectTargetedSentimentResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResultList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfDetectTargetedSentimentResult\"\n        },\n        {\n          \"description\": \"A list of objects containing the results of the operation. The results are sorted in ascending order by the <code>Index</code> field and match the order of the documents in the input list. If all of the documents contain an error, the <code>ResultList</code> is empty.\"\n        }\n      ]\n    },\n    \"ErrorList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchItemErrorList\"\
  \n        },\n        {\n          \"description\": \"List of errors that the operation can return.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResultList\",\n    \"ErrorList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-batch-detect-targeted-sentiment-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: BatchDetectTargetedSentimentResponse
---
