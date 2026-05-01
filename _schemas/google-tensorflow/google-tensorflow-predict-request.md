---
description: Schema for a prediction request to the TensorFlow Serving REST API, used to send input data for model inference.
layout: schema
name: TensorFlow Serving Predict Request
properties_list:
- description: The TensorFlow serving signature to invoke. Defaults to 'serving_default'.
  name: signature_name
  type: string
- description: A list of input instances in row format. Each instance is an object or value matching the model's input signature.
  name: instances
  type: array
- description: Input tensors in columnar format. Keys are input tensor names, values are the tensor data.
  name: inputs
  type: object
provider_name: Google TensorFlow
provider_slug: google-tensorflow
schema_file: json-schema/google-tensorflow-predict-request-schema.json
slug: google-tensorflow-predict-request
source_filename: google-tensorflow-predict-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.tensorflow.org/schemas/serving/predict-request.json\",\n  \"title\": \"TensorFlow Serving Predict Request\",\n  \"description\": \"Schema for a prediction request to the TensorFlow Serving REST API, used to send input data for model inference.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"signature_name\": {\n      \"type\": \"string\",\n      \"description\": \"The TensorFlow serving signature to invoke. Defaults to 'serving_default'.\",\n      \"default\": \"serving_default\"\n    },\n    \"instances\": {\n      \"type\": \"array\",\n      \"description\": \"A list of input instances in row format. Each instance is an object or value matching the model's input signature.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/InputInstance\"\n      }\n    },\n    \"inputs\": {\n      \"description\": \"Input tensors in columnar format. Keys are input tensor names, values are\
  \ the tensor data.\",\n      \"oneOf\": [\n        {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/TensorValue\"\n          }\n        }\n      ]\n    }\n  },\n  \"oneOf\": [\n    { \"required\": [\"instances\"] },\n    { \"required\": [\"inputs\"] }\n  ],\n  \"$defs\": {\n    \"InputInstance\": {\n      \"description\": \"A single input instance for prediction\",\n      \"oneOf\": [\n        { \"type\": \"number\" },\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": {} },\n        { \"type\": \"object\", \"additionalProperties\": true }\n      ]\n    },\n    \"TensorValue\": {\n      \"description\": \"A tensor value which can be a scalar, list, or nested list\",\n      \"oneOf\": [\n        { \"type\": \"number\" },\n        { \"type\": \"string\" },\n        { \"type\": \"boolean\" },\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/TensorValue\"\n\
  \          }\n        }\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tensorflow/refs/heads/main/json-schema/google-tensorflow-predict-request-schema.json
tags:
- AI
- Deep Learning
- Google
- Machine Learning
- Model Serving
- Open Source
title: TensorFlow Serving Predict Request
---
