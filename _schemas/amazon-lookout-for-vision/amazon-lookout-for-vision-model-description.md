---
description: Describes an Amazon Lookout for Vision model.
layout: schema
name: ModelDescription
properties_list:
- description: ''
  name: ModelVersion
  type: object
- description: ''
  name: ModelArn
  type: object
- description: ''
  name: CreationTimestamp
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
- description: ''
  name: Performance
  type: object
- description: ''
  name: OutputConfig
  type: object
- description: ''
  name: EvaluationManifest
  type: object
- description: ''
  name: EvaluationResult
  type: object
- description: ''
  name: EvaluationEndTimestamp
  type: object
- description: ''
  name: KmsKeyId
  type: object
- description: ''
  name: MinInferenceUnits
  type: object
- description: ''
  name: MaxInferenceUnits
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-model-description-schema.json
slug: amazon-lookout-for-vision-model-description
source_filename: amazon-lookout-for-vision-model-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-model-description-schema.json\",\n  \"title\": \"ModelDescription\",\n  \"description\": \"Describes an Amazon Lookout for Vision model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ModelVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelVersion\"\n        },\n        {\n          \"description\": \"The version of the model\"\n        }\n      ]\n    },\n    \"ModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the model.\"\n        }\n      ]\n    },\n    \"CreationTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n   \
  \     {\n          \"description\": \"The unix timestamp for the date and time that the model was created. \"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelDescriptionMessage\"\n        },\n        {\n          \"description\": \"The description for the model.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelStatus\"\n        },\n        {\n          \"description\": \"The status of the model.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelStatusMessage\"\n        },\n        {\n          \"description\": \"The status message for the model.\"\n        }\n      ]\n    },\n    \"Performance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelPerformance\"\n        },\n        {\n          \"description\"\
  : \"Performance metrics for the model. Created during training.\"\n        }\n      ]\n    },\n    \"OutputConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputConfig\"\n        },\n        {\n          \"description\": \"The S3 location where Amazon Lookout for Vision saves model training files.\"\n        }\n      ]\n    },\n    \"EvaluationManifest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputS3Object\"\n        },\n        {\n          \"description\": \"The S3 location where Amazon Lookout for Vision saves the manifest file that was used to test the trained model and generate the performance scores.\"\n        }\n      ]\n    },\n    \"EvaluationResult\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputS3Object\"\n        },\n        {\n          \"description\": \"The S3 location where Amazon Lookout for Vision saves the performance metrics.\"\n        }\n      ]\n\
  \    },\n    \"EvaluationEndTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The unix timestamp for the date and time that the evaluation ended. \"\n        }\n      ]\n    },\n    \"KmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyId\"\n        },\n        {\n          \"description\": \"The identifer for the AWS Key Management Service (AWS KMS) key that was used to encrypt the model during training.\"\n        }\n      ]\n    },\n    \"MinInferenceUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InferenceUnits\"\n        },\n        {\n          \"description\": \"The minimum number of inference units used by the model. For more information, see <a>StartModel</a> \"\n        }\n      ]\n    },\n    \"MaxInferenceUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InferenceUnits\"\
  \n        },\n        {\n          \"description\": \"The maximum number of inference units Amazon Lookout for Vision uses to auto-scale the model. For more information, see <a>StartModel</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-model-description-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: ModelDescription
---
