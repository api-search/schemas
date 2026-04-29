---
description: Schema for an Amazon Comprehend entity detection result, representing named entities identified in text through NLP analysis.
layout: schema
name: Amazon Comprehend Entity
properties_list:
- description: A collection of entities identified in the input text.
  name: Entities
  type: array
- description: The inferred sentiment detected in the input text.
  name: Sentiment
  type: string
- description: The confidence scores for each sentiment type.
  name: SentimentScore
  type: object
- description: A collection of key phrases identified in the input text.
  name: KeyPhrases
  type: array
- description: The languages detected in the input text.
  name: Languages
  type: array
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/amazon-comprehend-entity-schema.json
slug: amazon-comprehend-entity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://example.com/schemas/amazon-comprehend-entity.json\",\n  \"title\": \"Amazon Comprehend Entity\",\n  \"description\": \"Schema for an Amazon Comprehend entity detection result, representing named entities identified in text through NLP analysis.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Entities\": {\n      \"type\": \"array\",\n      \"description\": \"A collection of entities identified in the input text.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Entity\"\n      }\n    },\n    \"Sentiment\": {\n      \"type\": \"string\",\n      \"description\": \"The inferred sentiment detected in the input text.\",\n      \"enum\": [\"POSITIVE\", \"NEGATIVE\", \"NEUTRAL\", \"MIXED\"]\n    },\n    \"SentimentScore\": {\n      \"type\": \"object\",\n      \"description\": \"The confidence scores for each sentiment type.\",\n      \"properties\": {\n        \"Positive\": {\n   \
  \       \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 1\n        },\n        \"Negative\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 1\n        },\n        \"Neutral\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 1\n        },\n        \"Mixed\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 1\n        }\n      }\n    },\n    \"KeyPhrases\": {\n      \"type\": \"array\",\n      \"description\": \"A collection of key phrases identified in the input text.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/KeyPhrase\"\n      }\n    },\n    \"Languages\": {\n      \"type\": \"array\",\n      \"description\": \"The languages detected in the input text.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DominantLanguage\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Entity\": {\n      \"type\": \"object\",\n      \"description\": \"A named\
  \ entity identified in the text.\",\n      \"properties\": {\n        \"Score\": {\n          \"type\": \"number\",\n          \"description\": \"The level of confidence that Comprehend has in the accuracy of the detection.\",\n          \"minimum\": 0,\n          \"maximum\": 1\n        },\n        \"Type\": {\n          \"type\": \"string\",\n          \"description\": \"The entity type.\",\n          \"enum\": [\n            \"PERSON\",\n            \"LOCATION\",\n            \"ORGANIZATION\",\n            \"COMMERCIAL_ITEM\",\n            \"EVENT\",\n            \"DATE\",\n            \"QUANTITY\",\n            \"TITLE\",\n            \"OTHER\"\n          ]\n        },\n        \"Text\": {\n          \"type\": \"string\",\n          \"description\": \"The text of the entity.\"\n        },\n        \"BeginOffset\": {\n          \"type\": \"integer\",\n          \"description\": \"The zero-based offset in the input text where the entity begins.\",\n          \"minimum\": 0\n        },\n\
  \        \"EndOffset\": {\n          \"type\": \"integer\",\n          \"description\": \"The zero-based offset in the input text after the entity ends.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"KeyPhrase\": {\n      \"type\": \"object\",\n      \"description\": \"A key phrase detected in the text.\",\n      \"properties\": {\n        \"Score\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 1\n        },\n        \"Text\": {\n          \"type\": \"string\",\n          \"description\": \"The text of the key phrase.\"\n        },\n        \"BeginOffset\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        },\n        \"EndOffset\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"DominantLanguage\": {\n      \"type\": \"object\",\n      \"description\": \"A language detected in the text.\",\n      \"properties\": {\n        \"LanguageCode\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"The RFC 5646 language code for the dominant language.\"\n        },\n        \"Score\": {\n          \"type\": \"number\",\n          \"description\": \"The confidence score for the detected language.\",\n          \"minimum\": 0,\n          \"maximum\": 1\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/amazon-comprehend-entity-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: Amazon Comprehend Entity
---
