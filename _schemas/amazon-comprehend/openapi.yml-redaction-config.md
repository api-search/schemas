---
description: Provides configuration parameters for PII entity redaction.
layout: schema
name: RedactionConfig
properties_list:
- description: ''
  name: PiiEntityTypes
  type: object
- description: ''
  name: MaskMode
  type: object
- description: ''
  name: MaskCharacter
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-redaction-config-schema.json
slug: openapi.yml-redaction-config
source_filename: openapi.yml-redaction-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-redaction-config-schema.json\",\n  \"title\": \"RedactionConfig\",\n  \"description\": \"Provides configuration parameters for PII entity redaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PiiEntityTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfPiiEntityTypes\"\n        },\n        {\n          \"description\": \"An array of the types of PII entities that Amazon Comprehend detects in the input text for your request.\"\n        }\n      ]\n    },\n    \"MaskMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PiiEntitiesDetectionMaskMode\"\n        },\n        {\n          \"description\": \"Specifies whether the PII entity is redacted with the mask character or the entity type.\"\n        }\n    \
  \  ]\n    },\n    \"MaskCharacter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaskCharacter\"\n        },\n        {\n          \"description\": \"A character that replaces each character in the redacted PII entity.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-redaction-config-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: RedactionConfig
---
