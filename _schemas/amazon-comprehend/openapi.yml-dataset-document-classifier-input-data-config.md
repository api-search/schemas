---
description: <p>Describes the dataset input data configuration for a document classifier model.</p> <p>For more information on how the input file is formatted, see <a href="https://docs.aws.amazon.com/comprehend/latest/dg/prep-classifier-data.html">Preparing training data</a> in the Comprehend Developer Guide. </p>
layout: schema
name: DatasetDocumentClassifierInputDataConfig
properties_list:
- description: ''
  name: S3Uri
  type: object
- description: ''
  name: LabelDelimiter
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-dataset-document-classifier-input-data-config-schema.json
slug: openapi.yml-dataset-document-classifier-input-data-config
source_filename: openapi.yml-dataset-document-classifier-input-data-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-document-classifier-input-data-config-schema.json\",\n  \"title\": \"DatasetDocumentClassifierInputDataConfig\",\n  \"description\": \"<p>Describes the dataset input data configuration for a document classifier model.</p> <p>For more information on how the input file is formatted, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/prep-classifier-data.html\\\">Preparing training data</a> in the Comprehend Developer Guide. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"<p>The Amazon S3 URI for the input data. The S3 bucket must be in the same Region as the API endpoint that you are calling. The URI can point to\
  \ a single input file or it can provide the prefix for a collection of input files.</p> <p>For example, if you use the URI <code>S3://bucketName/prefix</code>, if the prefix is a single file, Amazon Comprehend uses that file as input. If more than one file begins with the prefix, Amazon Comprehend uses all of them as input.</p> <p>This parameter is required if you set <code>DataFormat</code> to <code>COMPREHEND_CSV</code>.</p>\"\n        }\n      ]\n    },\n    \"LabelDelimiter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LabelDelimiter\"\n        },\n        {\n          \"description\": \"Indicates the delimiter used to separate each label for training a multi-label classifier. The default delimiter between labels is a pipe (|). You can use a different character as a delimiter (if it's an allowed character) by specifying it under Delimiter for labels. If the training documents use a delimiter other than the default or the delimiter you specify, the\
  \ labels on that line will be combined to make a single unique label, such as LABELLABELLABEL.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3Uri\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-document-classifier-input-data-config-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DatasetDocumentClassifierInputDataConfig
---
