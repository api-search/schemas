---
description: CreateDatasetRequest schema
layout: schema
name: CreateDatasetRequest
properties_list:
- description: ''
  name: FlywheelArn
  type: object
- description: ''
  name: DatasetName
  type: object
- description: ''
  name: DatasetType
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: InputDataConfig
  type: object
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-create-dataset-request-schema.json
slug: openapi.yml-create-dataset-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-create-dataset-request-schema.json\",\n  \"title\": \"CreateDatasetRequest\",\n  \"description\": \"CreateDatasetRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlywheelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendFlywheelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the flywheel of the flywheel to receive the data.\"\n        }\n      ]\n    },\n    \"DatasetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArnName\"\n        },\n        {\n          \"description\": \"Name of the dataset.\"\n        }\n      ]\n    },\n    \"DatasetType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetType\"\
  \n        },\n        {\n          \"description\": \"The dataset type. You can specify that the data in a dataset is for training the model or for testing the model.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"Description of the dataset.\"\n        }\n      ]\n    },\n    \"InputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetInputDataConfig\"\n        },\n        {\n          \"description\": \"Information about the input data configuration. The type of input data varies based on the format of the input and whether the data is for a classifier model or an entity recognition model.\"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestTokenString\"\n        },\n        {\n          \"description\"\
  : \"A unique identifier for the request. If you don't set the client request token, Amazon Comprehend generates one.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Tags for the dataset.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FlywheelArn\",\n    \"DatasetName\",\n    \"InputDataConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-create-dataset-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: CreateDatasetRequest
---
