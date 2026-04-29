---
description: '<p>Provides configuration parameters to override the default actions for extracting text from PDF documents and image files. </p> <p> By default, Amazon Comprehend performs the following actions to extract text from files, based on the input file type: </p> <ul> <li> <p> <b>Word files</b> - Amazon Comprehend parser extracts the text. </p> </li> <li> <p> <b>Digital PDF files</b> - Amazon Comprehend parser extracts the text. </p> </li> <li> <p> <b>Image files and scanned PDF files</b> - Amazon Comprehend uses the Amazon Textract <code>DetectDocumentText</code> API to extract the text. </p> </li> </ul> <p> <code>DocumentReaderConfig</code> does not apply to plain text files or Word files.</p> <p> For image files and PDF documents, you can override these default actions using the fields listed below. For more information, see <a href="https://docs.aws.amazon.com/comprehend/latest/dg/idp-set-textract-options.html"> Setting text extraction options</a> in the Comprehend Developer
  Guide. </p>'
layout: schema
name: DocumentReaderConfig
properties_list:
- description: ''
  name: DocumentReadAction
  type: object
- description: ''
  name: DocumentReadMode
  type: object
- description: ''
  name: FeatureTypes
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-document-reader-config-schema.json
slug: openapi.yml-document-reader-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-reader-config-schema.json\",\n  \"title\": \"DocumentReaderConfig\",\n  \"description\": \"<p>Provides configuration parameters to override the default actions for extracting text from PDF documents and image files. </p> <p> By default, Amazon Comprehend performs the following actions to extract text from files, based on the input file type: </p> <ul> <li> <p> <b>Word files</b> - Amazon Comprehend parser extracts the text. </p> </li> <li> <p> <b>Digital PDF files</b> - Amazon Comprehend parser extracts the text. </p> </li> <li> <p> <b>Image files and scanned PDF files</b> - Amazon Comprehend uses the Amazon Textract <code>DetectDocumentText</code> API to extract the text. </p> </li> </ul> <p> <code>DocumentReaderConfig</code> does not apply to plain text files or Word files.</p>\
  \ <p> For image files and PDF documents, you can override these default actions using the fields listed below. For more information, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/idp-set-textract-options.html\\\"> Setting text extraction options</a> in the Comprehend Developer Guide. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocumentReadAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentReadAction\"\n        },\n        {\n          \"description\": \"<p>This field defines the Amazon Textract API operation that Amazon Comprehend uses to extract text from PDF files and image files. Enter one of the following values:</p> <ul> <li> <p> <code>TEXTRACT_DETECT_DOCUMENT_TEXT</code> - The Amazon Comprehend service uses the <code>DetectDocumentText</code> API operation. </p> </li> <li> <p> <code>TEXTRACT_ANALYZE_DOCUMENT</code> - The Amazon Comprehend service uses the <code>AnalyzeDocument</code> API operation. </p>\
  \ </li> </ul>\"\n        }\n      ]\n    },\n    \"DocumentReadMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentReadMode\"\n        },\n        {\n          \"description\": \"<p>Determines the text extraction actions for PDF files. Enter one of the following values:</p> <ul> <li> <p> <code>SERVICE_DEFAULT</code> - use the Amazon Comprehend service defaults for PDF files.</p> </li> <li> <p> <code>FORCE_DOCUMENT_READ_ACTION</code> - Amazon Comprehend uses the Textract API specified by DocumentReadAction for all PDF files, including digital PDF files. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"FeatureTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfDocumentReadFeatureTypes\"\n        },\n        {\n          \"description\": \"<p>Specifies the type of Amazon Textract features to apply. If you chose <code>TEXTRACT_ANALYZE_DOCUMENT</code> as the read action, you must specify one or both of the\
  \ following values:</p> <ul> <li> <p> <code>TABLES</code> - Returns information about any tables that are detected in the input document. </p> </li> <li> <p> <code>FORMS</code> - Returns information and the data from any forms that are detected in the input document. </p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DocumentReadAction\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-reader-config-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DocumentReaderConfig
---
