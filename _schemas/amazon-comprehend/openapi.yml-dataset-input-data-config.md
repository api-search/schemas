---
description: Specifies the format and location of the input data for the dataset.
layout: schema
name: DatasetInputDataConfig
properties_list:
- description: ''
  name: AugmentedManifests
  type: object
- description: ''
  name: DataFormat
  type: object
- description: ''
  name: DocumentClassifierInputDataConfig
  type: object
- description: ''
  name: EntityRecognizerInputDataConfig
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-dataset-input-data-config-schema.json
slug: openapi.yml-dataset-input-data-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-input-data-config-schema.json\",\n  \"title\": \"DatasetInputDataConfig\",\n  \"description\": \"Specifies the format and location of the input data for the dataset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AugmentedManifests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetAugmentedManifestsList\"\n        },\n        {\n          \"description\": \"A list of augmented manifest files that provide training data for your custom model. An augmented manifest file is a labeled dataset that is produced by Amazon SageMaker Ground Truth. \"\n        }\n      ]\n    },\n    \"DataFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetDataFormat\"\n        },\n        {\n          \"description\": \"\
  <p> <code>COMPREHEND_CSV</code>: The data format is a two-column CSV file, where the first column contains labels and the second column contains documents.</p> <p> <code>AUGMENTED_MANIFEST</code>: The data format </p>\"\n        }\n      ]\n    },\n    \"DocumentClassifierInputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetDocumentClassifierInputDataConfig\"\n        },\n        {\n          \"description\": \"<p>The input properties for training a document classifier model. </p> <p>For more information on how the input file is formatted, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/prep-classifier-data.html\\\">Preparing training data</a> in the Comprehend Developer Guide. </p>\"\n        }\n      ]\n    },\n    \"EntityRecognizerInputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetEntityRecognizerInputDataConfig\"\n        },\n        {\n          \"description\":\
  \ \"The input properties for training an entity recognizer model.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-input-data-config-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DatasetInputDataConfig
---
