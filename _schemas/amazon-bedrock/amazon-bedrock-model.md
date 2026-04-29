---
description: Schema representing an Amazon Bedrock foundation model and its capabilities.
layout: schema
name: Amazon Bedrock Foundation Model
properties_list:
- description: The Amazon Resource Name (ARN) of the foundation model.
  name: modelArn
  type: string
- description: The unique identifier for the foundation model (e.g., anthropic.claude-3-sonnet-20240229-v1:0).
  name: modelId
  type: string
- description: The display name of the foundation model.
  name: modelName
  type: string
- description: The name of the model provider.
  name: providerName
  type: string
- description: The input modalities supported by the model.
  name: inputModalities
  type: array
- description: The output modalities supported by the model.
  name: outputModalities
  type: array
- description: Whether the model supports response streaming.
  name: responseStreamingSupported
  type: boolean
- description: The customization types supported by the model.
  name: customizationsSupported
  type: array
- description: The inference types supported by the model.
  name: inferenceTypesSupported
  type: array
- description: Lifecycle information for the model.
  name: modelLifecycle
  type: object
provider_name: Amazon Bedrock
provider_slug: amazon-bedrock
schema_file: json-schema/amazon-bedrock-model-schema.json
slug: amazon-bedrock-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://aws.amazon.com/bedrock/schemas/foundation-model.json\",\n  \"title\": \"Amazon Bedrock Foundation Model\",\n  \"description\": \"Schema representing an Amazon Bedrock foundation model and its capabilities.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"modelId\",\n    \"modelName\",\n    \"providerName\"\n  ],\n  \"properties\": {\n    \"modelArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the foundation model.\",\n      \"pattern\": \"^arn:aws:bedrock:[a-z0-9-]+::foundation-model/.+$\"\n    },\n    \"modelId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the foundation model (e.g., anthropic.claude-3-sonnet-20240229-v1:0).\",\n      \"examples\": [\n        \"anthropic.claude-3-sonnet-20240229-v1:0\",\n        \"amazon.titan-text-express-v1\",\n        \"meta.llama3-70b-instruct-v1:0\"\n  \
  \    ]\n    },\n    \"modelName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the foundation model.\"\n    },\n    \"providerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the model provider.\",\n      \"examples\": [\n        \"Amazon\",\n        \"Anthropic\",\n        \"Meta\",\n        \"Cohere\",\n        \"AI21 Labs\",\n        \"Stability AI\",\n        \"Mistral AI\"\n      ]\n    },\n    \"inputModalities\": {\n      \"type\": \"array\",\n      \"description\": \"The input modalities supported by the model.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"TEXT\",\n          \"IMAGE\",\n          \"EMBEDDING\"\n        ]\n      }\n    },\n    \"outputModalities\": {\n      \"type\": \"array\",\n      \"description\": \"The output modalities supported by the model.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"TEXT\",\n          \"IMAGE\"\
  ,\n          \"EMBEDDING\"\n        ]\n      }\n    },\n    \"responseStreamingSupported\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the model supports response streaming.\"\n    },\n    \"customizationsSupported\": {\n      \"type\": \"array\",\n      \"description\": \"The customization types supported by the model.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"FINE_TUNING\",\n          \"CONTINUED_PRE_TRAINING\"\n        ]\n      }\n    },\n    \"inferenceTypesSupported\": {\n      \"type\": \"array\",\n      \"description\": \"The inference types supported by the model.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"ON_DEMAND\",\n          \"PROVISIONED\"\n        ]\n      }\n    },\n    \"modelLifecycle\": {\n      \"type\": \"object\",\n      \"description\": \"Lifecycle information for the model.\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The lifecycle status of the model.\",\n          \"enum\": [\n            \"ACTIVE\",\n            \"LEGACY\"\n          ]\n        }\n      }\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-bedrock/refs/heads/main/json-schema/amazon-bedrock-model-schema.json
tags:
- AI
- AWS
- Foundation Models
- Generative AI
- LLM
- Machine Learning
- RAG
- Agents
- Responsible AI
title: Amazon Bedrock Foundation Model
---
