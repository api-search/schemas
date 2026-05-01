---
description: Specifies the format and location of the input data.
layout: schema
name: EntityRecognizerInputDataConfig
properties_list:
- description: ''
  name: DataFormat
  type: object
- description: ''
  name: EntityTypes
  type: object
- description: ''
  name: Documents
  type: object
- description: ''
  name: Annotations
  type: object
- description: ''
  name: EntityList
  type: object
- description: ''
  name: AugmentedManifests
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-entity-recognizer-input-data-config-schema.json
slug: openapi.yml-entity-recognizer-input-data-config
source_filename: openapi.yml-entity-recognizer-input-data-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognizer-input-data-config-schema.json\",\n  \"title\": \"EntityRecognizerInputDataConfig\",\n  \"description\": \"Specifies the format and location of the input data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DataFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityRecognizerDataFormat\"\n        },\n        {\n          \"description\": \"<p>The format of your training data:</p> <ul> <li> <p> <code>COMPREHEND_CSV</code>: A CSV file that supplements your training documents. The CSV file contains information about the custom entities that your trained model will detect. The required format of the file depends on whether you are providing annotations or an entity list.</p> <p>If you use this value, you must provide your CSV file\
  \ by using either the <code>Annotations</code> or <code>EntityList</code> parameters. You must provide your training documents by using the <code>Documents</code> parameter.</p> </li> <li> <p> <code>AUGMENTED_MANIFEST</code>: A labeled dataset that is produced by Amazon SageMaker Ground Truth. This file is in JSON lines format. Each line is a complete JSON object that contains a training document and its labels. Each label annotates a named entity in the training document. </p> <p>If you use this value, you must provide the <code>AugmentedManifests</code> parameter in your request.</p> </li> </ul> <p>If you don't specify a value, Amazon Comprehend uses <code>COMPREHEND_CSV</code> as the default.</p>\"\n        }\n      ]\n    },\n    \"EntityTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityTypesList\"\n        },\n        {\n          \"description\": \"<p>The entity types in the labeled training data that Amazon Comprehend uses to train the custom\
  \ entity recognizer. Any entity types that you don't specify are ignored.</p> <p>A maximum of 25 entity types can be used at one time to train an entity recognizer. Entity types must not contain the following invalid characters: \\\\n (line break), \\\\\\\\n (escaped line break), \\\\r (carriage return), \\\\\\\\r (escaped carriage return), \\\\t (tab), \\\\\\\\t (escaped tab), space, and , (comma). </p>\"\n        }\n      ]\n    },\n    \"Documents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityRecognizerDocuments\"\n        },\n        {\n          \"description\": \"<p>The S3 location of the folder that contains the training documents for your custom entity recognizer.</p> <p>This parameter is required if you set <code>DataFormat</code> to <code>COMPREHEND_CSV</code>.</p>\"\n        }\n      ]\n    },\n    \"Annotations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityRecognizerAnnotations\"\n        },\n \
  \       {\n          \"description\": \"The S3 location of the CSV file that annotates your training documents.\"\n        }\n      ]\n    },\n    \"EntityList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityRecognizerEntityList\"\n        },\n        {\n          \"description\": \"The S3 location of the CSV file that has the entity list for your custom entity recognizer.\"\n        }\n      ]\n    },\n    \"AugmentedManifests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityRecognizerAugmentedManifestsList\"\n        },\n        {\n          \"description\": \"<p>A list of augmented manifest files that provide training data for your custom model. An augmented manifest file is a labeled dataset that is produced by Amazon SageMaker Ground Truth.</p> <p>This parameter is required if you set <code>DataFormat</code> to <code>AUGMENTED_MANIFEST</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"\
  EntityTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognizer-input-data-config-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EntityRecognizerInputDataConfig
---
