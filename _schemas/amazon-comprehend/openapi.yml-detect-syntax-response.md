---
description: DetectSyntaxResponse schema
layout: schema
name: DetectSyntaxResponse
properties_list:
- description: ''
  name: SyntaxTokens
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-detect-syntax-response-schema.json
slug: openapi.yml-detect-syntax-response
source_filename: openapi.yml-detect-syntax-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-syntax-response-schema.json\",\n  \"title\": \"DetectSyntaxResponse\",\n  \"description\": \"DetectSyntaxResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SyntaxTokens\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfSyntaxTokens\"\n        },\n        {\n          \"description\": \"A collection of syntax tokens describing the text. For each token, the response provides the text, the token type, where the text begins and ends, and the level of confidence that Amazon Comprehend has that the token is correct. For a list of token types, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/how-syntax.html\\\">Syntax</a> in the Comprehend Developer Guide. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-syntax-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DetectSyntaxResponse
---
