---
description: Open Inference Protocol V2 inference request submitted to a model serving endpoint via HTTP POST. Compatible with KServe, NVIDIA Triton, BentoML, and other OIP-compliant servers.
layout: schema
name: Inference Request
properties_list:
- description: Optional request identifier that will be echoed back in the response for correlation.
  name: id
  type: string
- description: Optional key/value parameters passed to the model's pre/post-processing pipeline.
  name: parameters
  type: object
- description: Input tensors for the inference request. Each tensor specifies its name, shape, datatype, and data.
  name: inputs
  type: array
- description: Optional list of output tensors to return. If omitted, all model outputs are returned.
  name: outputs
  type: array
provider_name: Scalable Inference Serving
provider_slug: scalable-inference-serving
schema_file: json-schema/kserve-inference-request-schema.json
slug: kserve-inference-request
source_filename: kserve-inference-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scalable-inference-serving/main/json-schema/kserve-inference-request-schema.json\",\n  \"title\": \"Inference Request\",\n  \"description\": \"Open Inference Protocol V2 inference request submitted to a model serving endpoint via HTTP POST. Compatible with KServe, NVIDIA Triton, BentoML, and other OIP-compliant servers.\",\n  \"type\": \"object\",\n  \"required\": [\"inputs\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Optional request identifier that will be echoed back in the response for correlation.\",\n      \"example\": \"req-a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Optional key/value parameters passed to the model's pre/post-processing pipeline.\",\n      \"additionalProperties\": true\n    },\n    \"inputs\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Input tensors for the inference request. Each tensor specifies its name, shape, datatype, and data.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/RequestInput\"\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"description\": \"Optional list of output tensors to return. If omitted, all model outputs are returned.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/RequestOutput\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"RequestInput\": {\n      \"type\": \"object\",\n      \"title\": \"Request Input\",\n      \"description\": \"A single named input tensor for an inference request.\",\n      \"required\": [\"name\", \"shape\", \"datatype\", \"data\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Tensor name as defined in the model's input specification.\"\n        },\n        \"shape\": {\n          \"type\":\
  \ \"array\",\n          \"description\": \"Shape of the tensor. Use -1 for variable-length or batch dimensions.\",\n          \"items\": {\"type\": \"integer\"},\n          \"example\": [1, 128]\n        },\n        \"datatype\": {\n          \"$ref\": \"#/$defs/TensorDatatype\"\n        },\n        \"parameters\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Optional tensor-level parameters.\"\n        },\n        \"data\": {\n          \"description\": \"Tensor data in row-major order. Nested arrays or flat array acceptable.\",\n          \"oneOf\": [\n            {\"type\": \"array\", \"items\": {}},\n            {\"type\": \"string\", \"description\": \"Base64-encoded binary data for the binary tensor data extension.\"}\n          ]\n        }\n      }\n    },\n    \"RequestOutput\": {\n      \"type\": \"object\",\n      \"title\": \"Request Output\",\n      \"description\": \"Specifies which model output tensor to include\
  \ in the response.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the output tensor to include in the response.\"\n        },\n        \"parameters\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        }\n      }\n    },\n    \"TensorDatatype\": {\n      \"type\": \"string\",\n      \"title\": \"Tensor Datatype\",\n      \"description\": \"Data type of a tensor per the Open Inference Protocol specification.\",\n      \"enum\": [\"BOOL\", \"UINT8\", \"UINT16\", \"UINT32\", \"UINT64\", \"INT8\", \"INT16\", \"INT32\", \"INT64\", \"FP16\", \"FP32\", \"FP64\", \"BYTES\", \"STRING\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalable-inference-serving/refs/heads/main/json-schema/kserve-inference-request-schema.json
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
title: Inference Request
---
