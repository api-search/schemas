---
description: ClassifyDocumentResponse schema
layout: schema
name: ClassifyDocumentResponse
properties_list:
- description: ''
  name: Classes
  type: object
- description: ''
  name: Labels
  type: object
- description: ''
  name: DocumentMetadata
  type: object
- description: ''
  name: DocumentType
  type: object
- description: ''
  name: Errors
  type: object
- description: ''
  name: Warnings
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-classify-document-response-schema.json
slug: openapi.yml-classify-document-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-classify-document-response-schema.json\",\n  \"title\": \"ClassifyDocumentResponse\",\n  \"description\": \"ClassifyDocumentResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Classes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfClasses\"\n        },\n        {\n          \"description\": \"The classes used by the document being analyzed. These are used for multi-class trained models. Individual classes are mutually exclusive and each document is expected to have only a single class assigned to it. For example, an animal can be a dog or a cat, but not both at the same time. \"\n        }\n      ]\n    },\n    \"Labels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfLabels\"\n        },\n   \
  \     {\n          \"description\": \"The labels used the document being analyzed. These are used for multi-label trained models. Individual labels represent different categories that are related in some manner and are not mutually exclusive. For example, a movie can be just an action movie, or it can be an action movie, a science fiction movie, and a comedy, all at the same time. \"\n        }\n      ]\n    },\n    \"DocumentMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentMetadata\"\n        },\n        {\n          \"description\": \"Extraction information about the document. This field is present in the response only if your request includes the <code>Byte</code> parameter. \"\n        }\n      ]\n    },\n    \"DocumentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfDocumentType\"\n        },\n        {\n          \"description\": \"The document type for each page in the input document. This\
  \ field is present in the response only if your request includes the <code>Byte</code> parameter. \"\n        }\n      ]\n    },\n    \"Errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfErrors\"\n        },\n        {\n          \"description\": \"Page-level errors that the system detected while processing the input document. The field is empty if the system encountered no errors.\"\n        }\n      ]\n    },\n    \"Warnings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfWarnings\"\n        },\n        {\n          \"description\": \"<p>Warnings detected while processing the input document. The response includes a warning if there is a mismatch between the input document type and the model type associated with the endpoint that you specified. The response can also include warnings for individual pages that have a mismatch. </p> <p>The field is empty if the system generated no warnings.</p>\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-classify-document-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ClassifyDocumentResponse
---
