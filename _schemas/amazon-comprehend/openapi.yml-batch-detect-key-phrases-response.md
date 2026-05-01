---
description: BatchDetectKeyPhrasesResponse schema
layout: schema
name: BatchDetectKeyPhrasesResponse
properties_list:
- description: ''
  name: ResultList
  type: object
- description: ''
  name: ErrorList
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-batch-detect-key-phrases-response-schema.json
slug: openapi.yml-batch-detect-key-phrases-response
source_filename: openapi.yml-batch-detect-key-phrases-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-batch-detect-key-phrases-response-schema.json\",\n  \"title\": \"BatchDetectKeyPhrasesResponse\",\n  \"description\": \"BatchDetectKeyPhrasesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResultList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfDetectKeyPhrasesResult\"\n        },\n        {\n          \"description\": \"A list of objects containing the results of the operation. The results are sorted in ascending order by the <code>Index</code> field and match the order of the documents in the input list. If all of the documents contain an error, the <code>ResultList</code> is empty.\"\n        }\n      ]\n    },\n    \"ErrorList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchItemErrorList\"\
  \n        },\n        {\n          \"description\": \"A list containing one object for each document that contained an error. The results are sorted in ascending order by the <code>Index</code> field and match the order of the documents in the input list. If there are no errors in the batch, the <code>ErrorList</code> is empty.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResultList\",\n    \"ErrorList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-batch-detect-key-phrases-response-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: BatchDetectKeyPhrasesResponse
---
