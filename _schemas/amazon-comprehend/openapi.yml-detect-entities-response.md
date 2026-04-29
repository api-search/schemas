---
description: DetectEntitiesResponse schema
layout: schema
name: DetectEntitiesResponse
properties_list:
- description: ''
  name: Entities
  type: object
- description: ''
  name: DocumentMetadata
  type: object
- description: ''
  name: DocumentType
  type: object
- description: ''
  name: Blocks
  type: object
- description: ''
  name: Errors
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-detect-entities-response-schema.json
slug: openapi.yml-detect-entities-response
source_filename: openapi.yml-detect-entities-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-entities-response-schema.json\",\n  \"title\": \"DetectEntitiesResponse\",\n  \"description\": \"DetectEntitiesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Entities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfEntities\"\n        },\n        {\n          \"description\": \"<p>A collection of entities identified in the input text. For each entity, the response provides the entity text, entity type, where the entity text begins and ends, and the level of confidence that Amazon Comprehend has in the detection. </p> <p>If your request uses a custom entity recognition model, Amazon Comprehend detects the entities that the model is trained to recognize. Otherwise, it detects the default entity types. For a list of default\
  \ entity types, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/how-entities.html\\\">Entities</a> in the Comprehend Developer Guide. </p>\"\n        }\n      ]\n    },\n    \"DocumentMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentMetadata\"\n        },\n        {\n          \"description\": \"Information about the document, discovered during text extraction. This field is present in the response only if your request used the <code>Byte</code> parameter. \"\n        }\n      ]\n    },\n    \"DocumentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfDocumentType\"\n        },\n        {\n          \"description\": \"The document type for each page in the input document. This field is present in the response only if your request used the <code>Byte</code> parameter. \"\n        }\n      ]\n    },\n    \"Blocks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfBlocks\"\
  \n        },\n        {\n          \"description\": \"<p>Information about each block of text in the input document. Blocks are nested. A page block contains a block for each line of text, which contains a block for each word. </p> <p>The <code>Block</code> content for a Word input document does not include a <code>Geometry</code> field.</p> <p>The <code>Block</code> field is not present in the response for plain-text inputs.</p>\"\n        }\n      ]\n    },\n    \"Errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfErrors\"\n        },\n        {\n          \"description\": \"Page-level errors that the system detected while processing the input document. The field is empty if the system encountered no errors.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-entities-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DetectEntitiesResponse
---
