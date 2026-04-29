---
description: The flywheel properties.
layout: schema
name: FlywheelProperties
properties_list:
- description: ''
  name: FlywheelArn
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
  name: DataLakeS3Uri
  type: object
- description: ''
  name: DataSecurityConfig
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: ModelType
  type: object
- description: ''
  name: Message
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: LastModifiedTime
  type: object
- description: ''
  name: LatestFlywheelIteration
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-flywheel-properties-schema.json
slug: openapi.yml-flywheel-properties
source_filename: openapi.yml-flywheel-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-flywheel-properties-schema.json\",\n  \"title\": \"FlywheelProperties\",\n  \"description\": \"The flywheel properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlywheelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendFlywheelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the flywheel.\"\n        }\n      ]\n    },\n    \"ActiveModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the active model version.\"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\
  \n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that grants Amazon Comprehend permission to access the flywheel data.\"\n        }\n      ]\n    },\n    \"TaskConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskConfig\"\n        },\n        {\n          \"description\": \"Configuration about the custom classifier associated with the flywheel.\"\n        }\n      ]\n    },\n    \"DataLakeS3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"Amazon S3 URI of the data lake location. \"\n        }\n      ]\n    },\n    \"DataSecurityConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSecurityConfig\"\n        },\n        {\n          \"description\": \"Data security configuration.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/FlywheelStatus\"\n        },\n        {\n          \"description\": \"The status of the flywheel.\"\n        }\n      ]\n    },\n    \"ModelType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelType\"\n        },\n        {\n          \"description\": \"Model type of the flywheel's model.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnyLengthString\"\n        },\n        {\n          \"description\": \"A description of the status of the flywheel.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Creation time of the flywheel.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n\
  \          \"description\": \"Last modified time for the flywheel.\"\n        }\n      ]\n    },\n    \"LatestFlywheelIteration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlywheelIterationId\"\n        },\n        {\n          \"description\": \"The most recent flywheel iteration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-flywheel-properties-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: FlywheelProperties
---
