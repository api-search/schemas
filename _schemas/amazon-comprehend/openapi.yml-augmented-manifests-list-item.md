---
description: An augmented manifest file that provides training data for your custom model. An augmented manifest file is a labeled dataset that is produced by Amazon SageMaker Ground Truth.
layout: schema
name: AugmentedManifestsListItem
properties_list:
- description: ''
  name: S3Uri
  type: object
- description: ''
  name: Split
  type: object
- description: ''
  name: AttributeNames
  type: object
- description: ''
  name: AnnotationDataS3Uri
  type: object
- description: ''
  name: SourceDocumentsS3Uri
  type: object
- description: ''
  name: DocumentType
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-augmented-manifests-list-item-schema.json
slug: openapi.yml-augmented-manifests-list-item
source_filename: openapi.yml-augmented-manifests-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-augmented-manifests-list-item-schema.json\",\n  \"title\": \"AugmentedManifestsListItem\",\n  \"description\": \"An augmented manifest file that provides training data for your custom model. An augmented manifest file is a labeled dataset that is produced by Amazon SageMaker Ground Truth.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The Amazon S3 location of the augmented manifest file.\"\n        }\n      ]\n    },\n    \"Split\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Split\"\n        },\n        {\n          \"description\": \"<p>The purpose of the data you've provided in the augmented manifest.\
  \ You can either train or test this data. If you don't specify, the default is train.</p> <p>TRAIN - all of the documents in the manifest will be used for training. If no test documents are provided, Amazon Comprehend will automatically reserve a portion of the training documents for testing.</p> <p> TEST - all of the documents in the manifest will be used for testing.</p>\"\n        }\n      ]\n    },\n    \"AttributeNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeNamesList\"\n        },\n        {\n          \"description\": \"<p>The JSON attribute that contains the annotations for your training documents. The number of attribute names that you specify depends on whether your augmented manifest file is the output of a single labeling job or a chained labeling job.</p> <p>If your file is the output of a single labeling job, specify the LabelAttributeName key that was used when the job was created in Ground Truth.</p> <p>If your file is the\
  \ output of a chained labeling job, specify the LabelAttributeName key for one or more jobs in the chain. Each LabelAttributeName key provides the annotations from an individual job.</p>\"\n        }\n      ]\n    },\n    \"AnnotationDataS3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The S3 prefix to the annotation files that are referred in the augmented manifest file.\"\n        }\n      ]\n    },\n    \"SourceDocumentsS3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The S3 prefix to the source files (PDFs) that are referred to in the augmented manifest file.\"\n        }\n      ]\n    },\n    \"DocumentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AugmentedManifestsDocumentTypeFormat\"\n        },\n        {\n          \"description\": \"<p>The type\
  \ of augmented manifest. PlainTextDocument or SemiStructuredDocument. If you don't specify, the default is PlainTextDocument. </p> <ul> <li> <p> <code>PLAIN_TEXT_DOCUMENT</code> A document type that represents any unicode text that is encoded in UTF-8.</p> </li> <li> <p> <code>SEMI_STRUCTURED_DOCUMENT</code> A document type with positional and structural context, like a PDF. For training with Amazon Comprehend, only PDFs are supported. For inference, Amazon Comprehend support PDFs, DOCX and TXT.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3Uri\",\n    \"AttributeNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-augmented-manifests-list-item-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: AugmentedManifestsListItem
---
