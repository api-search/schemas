---
description: CreateFlywheelRequest schema
layout: schema
name: CreateFlywheelRequest
properties_list:
- description: ''
  name: FlywheelName
  type: object
- description: ''
  name: ActiveModelArn
  type: object
- description: ''
  name: DataAccessRoleArn
  type: object
- description: ''
  name: TaskConfig
  type: object
- description: ''
  name: ModelType
  type: object
- description: ''
  name: DataLakeS3Uri
  type: object
- description: ''
  name: DataSecurityConfig
  type: object
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-create-flywheel-request-schema.json
slug: openapi.yml-create-flywheel-request
source_filename: openapi.yml-create-flywheel-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-create-flywheel-request-schema.json\",\n  \"title\": \"CreateFlywheelRequest\",\n  \"description\": \"CreateFlywheelRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlywheelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArnName\"\n        },\n        {\n          \"description\": \"Name for the flywheel.\"\n        }\n      ]\n    },\n    \"ActiveModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"To associate an existing model with the flywheel, specify the Amazon Resource Number (ARN) of the model version.\"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that grants Amazon Comprehend the permissions required to access the flywheel data in the data lake.\"\n        }\n      ]\n    },\n    \"TaskConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskConfig\"\n        },\n        {\n          \"description\": \"Configuration about the custom classifier associated with the flywheel.\"\n        }\n      ]\n    },\n    \"ModelType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelType\"\n        },\n        {\n          \"description\": \"The model type.\"\n        }\n      ]\n    },\n    \"DataLakeS3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlywheelS3Uri\"\n        },\n        {\n          \"description\": \"Enter the S3 location for the data lake. You can specify a new S3 bucket or a new\
  \ folder of an existing S3 bucket. The flywheel creates the data lake at this location.\"\n        }\n      ]\n    },\n    \"DataSecurityConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSecurityConfig\"\n        },\n        {\n          \"description\": \"Data security configurations.\"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestTokenString\"\n        },\n        {\n          \"description\": \"A unique identifier for the request. If you don't set the client request token, Amazon Comprehend generates one.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags to associate with this flywheel.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FlywheelName\",\n    \"DataAccessRoleArn\",\n    \"DataLakeS3Uri\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-create-flywheel-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: CreateFlywheelRequest
---
