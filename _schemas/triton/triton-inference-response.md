---
description: An inference response returned by NVIDIA Triton Inference Server following the KServe V2 inference protocol. Contains the model identification, request correlation ID, and output tensors with their data.
layout: schema
name: Triton Inference Response
properties_list:
- description: Unique identifier for the response, matching the corresponding request ID
  name: id
  type: string
- description: Name of the model that produced the inference results
  name: model_name
  type: string
- description: Version of the model that produced the inference results
  name: model_version
  type: string
- description: Response-level parameters returned by the server
  name: parameters
  type: object
- description: Output tensors produced by the inference
  name: outputs
  type: array
provider_name: Triton Inference Server
provider_slug: triton
schema_file: json-schema/triton-inference-response-schema.json
slug: triton-inference-response
source_filename: triton-inference-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.nvidia.com/schemas/triton/inference-response.json\",\n  \"title\": \"Triton Inference Response\",\n  \"description\": \"An inference response returned by NVIDIA Triton Inference Server following the KServe V2 inference protocol. Contains the model identification, request correlation ID, and output tensors with their data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the response, matching the corresponding request ID\"\n    },\n    \"model_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the model that produced the inference results\"\n    },\n    \"model_version\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the model that produced the inference results\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Response-level parameters returned by the server\",\n      \"properties\": {\n        \"sequence_id\": {\n          \"oneOf\": [\n            { \"type\": \"integer\" },\n            { \"type\": \"string\" }\n          ],\n          \"description\": \"Sequence identifier if this response is part of a sequence\"\n        },\n        \"sequence_start\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates this is the first response in a sequence\"\n        },\n        \"sequence_end\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates this is the last response in a sequence\"\n        }\n      },\n      \"additionalProperties\": {\n        \"oneOf\": [\n          { \"type\": \"string\" },\n          { \"type\": \"boolean\" },\n          { \"type\": \"integer\" }\n        ]\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"description\": \"Output tensors produced by the inference\",\n      \"items\": {\n        \"\
  $ref\": \"#/$defs/OutputTensor\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"OutputTensor\": {\n      \"type\": \"object\",\n      \"description\": \"An output tensor returned by the model after inference\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the output tensor\"\n        },\n        \"shape\": {\n          \"type\": \"array\",\n          \"description\": \"Shape of the output tensor\",\n          \"items\": {\n            \"type\": \"integer\",\n            \"minimum\": 0\n          }\n        },\n        \"datatype\": {\n          \"type\": \"string\",\n          \"description\": \"Data type of the tensor elements\",\n          \"enum\": [\n            \"BOOL\",\n            \"UINT8\",\n            \"UINT16\",\n            \"UINT32\",\n            \"UINT64\",\n            \"INT8\",\n            \"INT16\",\n            \"INT32\",\n            \"INT64\",\n            \"FP16\",\n            \"FP32\",\n   \
  \         \"FP64\",\n            \"BYTES\",\n            \"BF16\"\n          ]\n        },\n        \"parameters\": {\n          \"type\": \"object\",\n          \"description\": \"Per-output parameters\",\n          \"properties\": {\n            \"binary_data_size\": {\n              \"type\": \"integer\",\n              \"minimum\": 0,\n              \"description\": \"Size in bytes of binary data appended after the JSON response body\"\n            }\n          },\n          \"additionalProperties\": {\n            \"oneOf\": [\n              { \"type\": \"string\" },\n              { \"type\": \"boolean\" },\n              { \"type\": \"integer\" }\n            ]\n          }\n        },\n        \"data\": {\n          \"type\": \"array\",\n          \"description\": \"Tensor data as a flattened row-major array of values\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/triton/refs/heads/main/json-schema/triton-inference-response-schema.json
tags:
- AI
- Deep Learning
- Inference
- Machine Learning
- Model Serving
title: Triton Inference Response
---
