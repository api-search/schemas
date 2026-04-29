---
description: <p>Information about one mention of an entity. The mention information includes the location of the mention in the text and the sentiment of the mention.</p> <p>For more information about targeted sentiment, see <a href="https://docs.aws.amazon.com/comprehend/latest/dg/how-targeted-sentiment.html">Targeted sentiment</a>.</p>
layout: schema
name: TargetedSentimentMention
properties_list:
- description: ''
  name: Score
  type: object
- description: ''
  name: GroupScore
  type: object
- description: ''
  name: Text
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: MentionSentiment
  type: object
- description: ''
  name: BeginOffset
  type: object
- description: ''
  name: EndOffset
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-targeted-sentiment-mention-schema.json
slug: openapi.yml-targeted-sentiment-mention
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-targeted-sentiment-mention-schema.json\",\n  \"title\": \"TargetedSentimentMention\",\n  \"description\": \"<p>Information about one mention of an entity. The mention information includes the location of the mention in the text and the sentiment of the mention.</p> <p>For more information about targeted sentiment, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/how-targeted-sentiment.html\\\">Targeted sentiment</a>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"Model confidence that the entity is relevant. Value range is zero to one, where one is highest confidence.\"\n        }\n      ]\n    },\n    \"GroupScore\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The confidence that all the entities mentioned in the group relate to the same entity.\"\n        }\n      ]\n    },\n    \"Text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The text in the document that identifies the entity.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetedSentimentEntityType\"\n        },\n        {\n          \"description\": \"The type of the entity. Amazon Comprehend supports a variety of <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/how-targeted-sentiment.html#how-targeted-sentiment-entities\\\">entity types</a>.\"\n        }\n      ]\n    },\n    \"MentionSentiment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MentionSentiment\"\
  \n        },\n        {\n          \"description\": \"Contains the sentiment and sentiment score for the mention.\"\n        }\n      ]\n    },\n    \"BeginOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The offset into the document text where the mention begins.\"\n        }\n      ]\n    },\n    \"EndOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The offset into the document text where the mention ends.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-targeted-sentiment-mention-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: TargetedSentimentMention
---
