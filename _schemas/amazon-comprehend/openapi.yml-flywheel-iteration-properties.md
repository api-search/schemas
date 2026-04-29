---
description: The configuration properties of a flywheel iteration.
layout: schema
name: FlywheelIterationProperties
properties_list:
- description: ''
  name: FlywheelArn
  type: object
- description: ''
  name: FlywheelIterationId
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Message
  type: object
- description: ''
  name: EvaluatedModelArn
  type: object
- description: ''
  name: EvaluatedModelMetrics
  type: object
- description: ''
  name: TrainedModelArn
  type: object
- description: ''
  name: TrainedModelMetrics
  type: object
- description: ''
  name: EvaluationManifestS3Prefix
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-flywheel-iteration-properties-schema.json
slug: openapi.yml-flywheel-iteration-properties
source_filename: openapi.yml-flywheel-iteration-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-flywheel-iteration-properties-schema.json\",\n  \"title\": \"FlywheelIterationProperties\",\n  \"description\": \"The configuration properties of a flywheel iteration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlywheelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendFlywheelArn\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"FlywheelIterationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlywheelIterationId\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\"\
  : \"The creation start time of the flywheel iteration.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The completion time of this flywheel iteration.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlywheelIterationStatus\"\n        },\n        {\n          \"description\": \"The status of the flywheel iteration.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnyLengthString\"\n        },\n        {\n          \"description\": \"A description of the status of the flywheel iteration.\"\n        }\n      ]\n    },\n    \"EvaluatedModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"The ARN\
  \ of the evaluated model associated with this flywheel iteration.\"\n        }\n      ]\n    },\n    \"EvaluatedModelMetrics\": {\n      \"$ref\": \"#/components/schemas/FlywheelModelEvaluationMetrics\"\n    },\n    \"TrainedModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"The ARN of the trained model associated with this flywheel iteration.\"\n        }\n      ]\n    },\n    \"TrainedModelMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlywheelModelEvaluationMetrics\"\n        },\n        {\n          \"description\": \"The metrics associated with the trained model.\"\n        }\n      ]\n    },\n    \"EvaluationManifestS3Prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-flywheel-iteration-properties-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: FlywheelIterationProperties
---
