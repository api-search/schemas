---
description: DetectEntitiesRequest schema
layout: schema
name: DetectEntitiesRequest
properties_list:
- description: ''
  name: Text
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: EndpointArn
  type: object
- description: ''
  name: Bytes
  type: object
- description: ''
  name: DocumentReaderConfig
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-detect-entities-request-schema.json
slug: openapi.yml-detect-entities-request
source_filename: openapi.yml-detect-entities-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-entities-request-schema.json\",\n  \"title\": \"DetectEntitiesRequest\",\n  \"description\": \"DetectEntitiesRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerInputString\"\n        },\n        {\n          \"description\": \"A UTF-8 text string. The maximum string size is 100 KB. If you enter text using this parameter, do not use the <code>Bytes</code> parameter.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\": \"<p>The language of the input documents. You can specify any of the primary languages supported by Amazon Comprehend.\
  \ If your request includes the endpoint for a custom entity recognition model, Amazon Comprehend uses the language of your custom model, and it ignores any language code that you specify here.</p> <p>All input documents must be in the same language.</p>\"\n        }\n      ]\n    },\n    \"EndpointArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityRecognizerEndpointArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name of an endpoint that is associated with a custom entity recognition model. Provide an endpoint if you want to detect entities by using your own custom model instead of the default model that is used by Amazon Comprehend.</p> <p>If you specify an endpoint, Amazon Comprehend uses the language of your custom model, and it ignores any language code that you provide in your request.</p> <p>For information about endpoints, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/manage-endpoints.html\\\
  \">Managing endpoints</a>.</p>\"\n        }\n      ]\n    },\n    \"Bytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SemiStructuredDocumentBlob\"\n        },\n        {\n          \"description\": \"<p>This field applies only when you use a custom entity recognition model that was trained with PDF annotations. For other cases, enter your text input in the <code>Text</code> field.</p> <p> Use the <code>Bytes</code> parameter to input a text, PDF, Word or image file. Using a plain-text file in the <code>Bytes</code> parameter is equivelent to using the <code>Text</code> parameter (the <code>Entities</code> field in the response is identical).</p> <p>You can also use the <code>Bytes</code> parameter to input an Amazon Textract <code>DetectDocumentText</code> or <code>AnalyzeDocument</code> output file.</p> <p>Provide the input document as a sequence of base64-encoded bytes. If your code uses an Amazon Web Services SDK to detect entities, the SDK may encode\
  \ the document file bytes for you. </p> <p>The maximum length of this field depends on the input document type. For details, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/idp-inputs-sync.html\\\"> Inputs for real-time custom analysis</a> in the Comprehend Developer Guide. </p> <p>If you use the <code>Bytes</code> parameter, do not use the <code>Text</code> parameter.</p>\"\n        }\n      ]\n    },\n    \"DocumentReaderConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentReaderConfig\"\n        },\n        {\n          \"description\": \"Provides configuration parameters to override the default actions for extracting text from PDF documents and image files.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-entities-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DetectEntitiesRequest
---
