---
description: <p>Information about one of the entities found by targeted sentiment analysis.</p> <p>For more information about targeted sentiment, see <a href="https://docs.aws.amazon.com/comprehend/latest/dg/how-targeted-sentiment.html">Targeted sentiment</a>.</p>
layout: schema
name: TargetedSentimentEntity
properties_list:
- description: ''
  name: DescriptiveMentionIndex
  type: object
- description: ''
  name: Mentions
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-targeted-sentiment-entity-schema.json
slug: openapi.yml-targeted-sentiment-entity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-targeted-sentiment-entity-schema.json\",\n  \"title\": \"TargetedSentimentEntity\",\n  \"description\": \"<p>Information about one of the entities found by targeted sentiment analysis.</p> <p>For more information about targeted sentiment, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/how-targeted-sentiment.html\\\">Targeted sentiment</a>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DescriptiveMentionIndex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfDescriptiveMentionIndices\"\n        },\n        {\n          \"description\": \"One or more index into the Mentions array that provides the best name for the entity group.\"\n        }\n      ]\n    },\n    \"Mentions\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/ListOfMentions\"\n        },\n        {\n          \"description\": \"An array of mentions of the entity in the document. The array represents a co-reference group. See <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/how-targeted-sentiment.html#how-targeted-sentiment-values\\\"> Co-reference group</a> for an example. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-targeted-sentiment-entity-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: TargetedSentimentEntity
---
