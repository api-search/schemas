---
description: Properties associated with the dataset.
layout: schema
name: DatasetProperties
properties_list:
- description: ''
  name: DatasetArn
  type: object
- description: ''
  name: DatasetName
  type: object
- description: ''
  name: DatasetType
  type: object
- description: ''
  name: DatasetS3Uri
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Message
  type: object
- description: ''
  name: NumberOfDocuments
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: EndTime
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-dataset-properties-schema.json
slug: openapi.yml-dataset-properties
source_filename: openapi.yml-dataset-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-properties-schema.json\",\n  \"title\": \"DatasetProperties\",\n  \"description\": \"Properties associated with the dataset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendDatasetArn\"\n        },\n        {\n          \"description\": \"The ARN of the dataset.\"\n        }\n      ]\n    },\n    \"DatasetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArnName\"\n        },\n        {\n          \"description\": \"The name of the dataset.\"\n        }\n      ]\n    },\n    \"DatasetType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetType\"\n        },\n        {\n          \"description\"\
  : \"The dataset type (training data or test data).\"\n        }\n      ]\n    },\n    \"DatasetS3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The S3 URI where the dataset is stored.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"Description of the dataset.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetStatus\"\n        },\n        {\n          \"description\": \"The dataset status. While the system creates the dataset, the status is <code>CREATING</code>. When the dataset is ready to use, the status changes to <code>COMPLETED</code>. \"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnyLengthString\"\
  \n        },\n        {\n          \"description\": \"A description of the status of the dataset.\"\n        }\n      ]\n    },\n    \"NumberOfDocuments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumberOfDocuments\"\n        },\n        {\n          \"description\": \"The number of documents in the dataset.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Creation time of the dataset.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Time when the data from the dataset becomes available in the data lake.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-properties-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DatasetProperties
---
