---
description: Metadata about a deployed model in an OIP-compliant inference server. Describes the model's name, available versions, serving platform, and input/output tensor specifications.
layout: schema
name: Model Metadata
properties_list:
- description: Name of the model as registered in the inference server.
  name: name
  type: string
- description: List of available model versions. May be empty if versioning is not supported.
  name: versions
  type: array
- description: Backend serving platform and framework.
  name: platform
  type: string
- description: Input tensor specifications for the model.
  name: inputs
  type: array
- description: Output tensor specifications for the model.
  name: outputs
  type: array
provider_name: Scalable Inference Serving
provider_slug: scalable-inference-serving
schema_file: json-schema/kserve-model-metadata-schema.json
slug: kserve-model-metadata
source_filename: kserve-model-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scalable-inference-serving/main/json-schema/kserve-model-metadata-schema.json\",\n  \"title\": \"Model Metadata\",\n  \"description\": \"Metadata about a deployed model in an OIP-compliant inference server. Describes the model's name, available versions, serving platform, and input/output tensor specifications.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"platform\", \"inputs\", \"outputs\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the model as registered in the inference server.\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"description\": \"List of available model versions. May be empty if versioning is not supported.\",\n      \"items\": {\"type\": \"string\"}\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"Backend\
  \ serving platform and framework.\",\n      \"examples\": [\n        \"tensorflow_savedmodel\",\n        \"pytorch_libtorch\",\n        \"sklearn_sklearn\",\n        \"xgboost_xgboost\",\n        \"onnxruntime_onnx\",\n        \"ensemble\",\n        \"vllm\",\n        \"python\"\n      ]\n    },\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"Input tensor specifications for the model.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TensorMetadata\"\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"description\": \"Output tensor specifications for the model.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TensorMetadata\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"TensorMetadata\": {\n      \"type\": \"object\",\n      \"title\": \"Tensor Metadata\",\n      \"description\": \"Specification of a single input or output tensor.\",\n      \"required\": [\"name\", \"datatype\", \"shape\"],\n      \"properties\": {\n        \"name\":\
  \ {\n          \"type\": \"string\",\n          \"description\": \"Tensor name.\"\n        },\n        \"datatype\": {\n          \"type\": \"string\",\n          \"description\": \"Data type (BOOL, INT32, FP32, BYTES, etc.)\",\n          \"enum\": [\"BOOL\", \"UINT8\", \"UINT16\", \"UINT32\", \"UINT64\", \"INT8\", \"INT16\", \"INT32\", \"INT64\", \"FP16\", \"FP32\", \"FP64\", \"BYTES\", \"STRING\"]\n        },\n        \"shape\": {\n          \"type\": \"array\",\n          \"description\": \"Tensor shape. -1 indicates a dynamic dimension.\",\n          \"items\": {\"type\": \"integer\"},\n          \"example\": [-1, 224, 224, 3]\n        },\n        \"parameters\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Optional tensor-specific parameters.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalable-inference-serving/refs/heads/main/json-schema/kserve-model-metadata-schema.json
tags:
- AI
- CNCF
- Deployment
- Inference
- Kubernetes
- LLM
- Machine Learning
- Model Serving
- MLOps
- Scalability
title: Model Metadata
---
