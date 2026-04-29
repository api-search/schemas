---
description: Identifies the part of speech represented by the token and gives the confidence that Amazon Comprehend has that the part of speech was correctly identified. For more information about the parts of speech that Amazon Comprehend can identify, see <a href="https://docs.aws.amazon.com/comprehend/latest/dg/how-syntax.html">Syntax</a> in the Comprehend Developer Guide.
layout: schema
name: PartOfSpeechTag
properties_list:
- description: ''
  name: Tag
  type: object
- description: ''
  name: Score
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-part-of-speech-tag-schema.json
slug: openapi.yml-part-of-speech-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-part-of-speech-tag-schema.json\",\n  \"title\": \"PartOfSpeechTag\",\n  \"description\": \"Identifies the part of speech represented by the token and gives the confidence that Amazon Comprehend has that the part of speech was correctly identified. For more information about the parts of speech that Amazon Comprehend can identify, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/how-syntax.html\\\">Syntax</a> in the Comprehend Developer Guide. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PartOfSpeechTagType\"\n        },\n        {\n          \"description\": \"Identifies the part of speech that the token represents.\"\n        }\n      ]\n    },\n    \"Score\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The confidence that Amazon Comprehend has that the part of speech was correctly identified.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-part-of-speech-tag-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: PartOfSpeechTag
---
