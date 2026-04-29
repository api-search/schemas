---
description: <p>The input properties for training a document classifier. </p> <p>For more information on how the input file is formatted, see <a href="https://docs.aws.amazon.com/comprehend/latest/dg/prep-classifier-data.html">Preparing training data</a> in the Comprehend Developer Guide. </p>
layout: schema
name: DocumentClassifierInputDataConfig
properties_list:
- description: ''
  name: DataFormat
  type: object
- description: ''
  name: S3Uri
  type: object
- description: ''
  name: TestS3Uri
  type: object
- description: ''
  name: LabelDelimiter
  type: object
- description: ''
  name: AugmentedManifests
  type: object
- description: ''
  name: DocumentType
  type: object
- description: ''
  name: Documents
  type: object
- description: ''
  name: DocumentReaderConfig
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-document-classifier-input-data-config-schema.json
slug: openapi.yml-document-classifier-input-data-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-classifier-input-data-config-schema.json\",\n  \"title\": \"DocumentClassifierInputDataConfig\",\n  \"description\": \"<p>The input properties for training a document classifier. </p> <p>For more information on how the input file is formatted, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/prep-classifier-data.html\\\">Preparing training data</a> in the Comprehend Developer Guide. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DataFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierDataFormat\"\n        },\n        {\n          \"description\": \"<p>The format of your training data:</p> <ul> <li> <p> <code>COMPREHEND_CSV</code>: A two-column CSV file, where labels are provided in the first column,\
  \ and documents are provided in the second. If you use this value, you must provide the <code>S3Uri</code> parameter in your request.</p> </li> <li> <p> <code>AUGMENTED_MANIFEST</code>: A labeled dataset that is produced by Amazon SageMaker Ground Truth. This file is in JSON lines format. Each line is a complete JSON object that contains a training document and its associated labels. </p> <p>If you use this value, you must provide the <code>AugmentedManifests</code> parameter in your request.</p> </li> </ul> <p>If you don't specify a value, Amazon Comprehend uses <code>COMPREHEND_CSV</code> as the default.</p>\"\n        }\n      ]\n    },\n    \"S3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"<p>The Amazon S3 URI for the input data. The S3 bucket must be in the same Region as the API endpoint that you are calling. The URI can point to a single input file or it can provide the prefix for\
  \ a collection of input files.</p> <p>For example, if you use the URI <code>S3://bucketName/prefix</code>, if the prefix is a single file, Amazon Comprehend uses that file as input. If more than one file begins with the prefix, Amazon Comprehend uses all of them as input.</p> <p>This parameter is required if you set <code>DataFormat</code> to <code>COMPREHEND_CSV</code>.</p>\"\n        }\n      ]\n    },\n    \"TestS3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"This specifies the Amazon S3 location where the test annotations for an entity recognizer are located. The URI must be in the same Amazon Web Services Region as the API endpoint that you are calling. \"\n        }\n      ]\n    },\n    \"LabelDelimiter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LabelDelimiter\"\n        },\n        {\n          \"description\": \"Indicates the delimiter used to\
  \ separate each label for training a multi-label classifier. The default delimiter between labels is a pipe (|). You can use a different character as a delimiter (if it's an allowed character) by specifying it under Delimiter for labels. If the training documents use a delimiter other than the default or the delimiter you specify, the labels on that line will be combined to make a single unique label, such as LABELLABELLABEL.\"\n        }\n      ]\n    },\n    \"AugmentedManifests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierAugmentedManifestsList\"\n        },\n        {\n          \"description\": \"<p>A list of augmented manifest files that provide training data for your custom model. An augmented manifest file is a labeled dataset that is produced by Amazon SageMaker Ground Truth.</p> <p>This parameter is required if you set <code>DataFormat</code> to <code>AUGMENTED_MANIFEST</code>.</p>\"\n        }\n      ]\n    },\n    \"DocumentType\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierDocumentTypeFormat\"\n        },\n        {\n          \"description\": \"The type of input documents for training the model. Provide plain-text documents to create a plain-text model, and provide semi-structured documents to create a native model.\"\n        }\n      ]\n    },\n    \"Documents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierDocuments\"\n        },\n        {\n          \"description\": \"The S3 location of the training documents. This parameter is required in a request to create a native classifier model.\"\n        }\n      ]\n    },\n    \"DocumentReaderConfig\": {\n      \"$ref\": \"#/components/schemas/DocumentReaderConfig\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-classifier-input-data-config-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DocumentClassifierInputDataConfig
---
