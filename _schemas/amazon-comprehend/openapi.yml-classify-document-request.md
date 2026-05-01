---
description: ClassifyDocumentRequest schema
layout: schema
name: ClassifyDocumentRequest
properties_list:
- description: ''
  name: Text
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
schema_file: json-schema/openapi.yml-classify-document-request-schema.json
slug: openapi.yml-classify-document-request
source_filename: openapi.yml-classify-document-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-classify-document-request-schema.json\",\n  \"title\": \"ClassifyDocumentRequest\",\n  \"description\": \"ClassifyDocumentRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerInputString\"\n        },\n        {\n          \"description\": \"The document text to be analyzed. If you enter text using this parameter, do not use the <code>Bytes</code> parameter.\"\n        }\n      ]\n    },\n    \"EndpointArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierEndpointArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the endpoint. For information about endpoints, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/manage-endpoints.html\\\
  \">Managing endpoints</a>.\"\n        }\n      ]\n    },\n    \"Bytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SemiStructuredDocumentBlob\"\n        },\n        {\n          \"description\": \"<p>Use the <code>Bytes</code> parameter to input a text, PDF, Word or image file. You can also use the <code>Bytes</code> parameter to input an Amazon Textract <code>DetectDocumentText</code> or <code>AnalyzeDocument</code> output file.</p> <p>Provide the input document as a sequence of base64-encoded bytes. If your code uses an Amazon Web Services SDK to classify documents, the SDK may encode the document file bytes for you. </p> <p>The maximum length of this field depends on the input document type. For details, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/idp-inputs-sync.html\\\"> Inputs for real-time custom analysis</a> in the Comprehend Developer Guide. </p> <p>If you use the <code>Bytes</code> parameter, do not use the <code>Text</code>\
  \ parameter.</p>\"\n        }\n      ]\n    },\n    \"DocumentReaderConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentReaderConfig\"\n        },\n        {\n          \"description\": \"Provides configuration parameters to override the default actions for extracting text from PDF documents and image files.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-classify-document-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ClassifyDocumentRequest
---
