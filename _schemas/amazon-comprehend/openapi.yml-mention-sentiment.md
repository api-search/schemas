---
description: <p>Contains the sentiment and sentiment score for one mention of an entity.</p> <p>For more information about targeted sentiment, see <a href="https://docs.aws.amazon.com/comprehend/latest/dg/how-targeted-sentiment.html">Targeted sentiment</a>.</p>
layout: schema
name: MentionSentiment
properties_list:
- description: ''
  name: Sentiment
  type: object
- description: ''
  name: SentimentScore
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-mention-sentiment-schema.json
slug: openapi.yml-mention-sentiment
source_filename: openapi.yml-mention-sentiment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-mention-sentiment-schema.json\",\n  \"title\": \"MentionSentiment\",\n  \"description\": \"<p>Contains the sentiment and sentiment score for one mention of an entity.</p> <p>For more information about targeted sentiment, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/how-targeted-sentiment.html\\\">Targeted sentiment</a>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Sentiment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SentimentType\"\n        },\n        {\n          \"description\": \"The sentiment of the mention. \"\n        }\n      ]\n    },\n    \"SentimentScore\": {\n      \"$ref\": \"#/components/schemas/SentimentScore\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-mention-sentiment-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: MentionSentiment
---
