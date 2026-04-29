---
description: Endpoint schema from Amazon SageMaker API
layout: schema
name: Endpoint
properties_list:
- description: The name of the endpoint.
  name: EndpointName
  type: string
- description: The Amazon Resource Name (ARN) of the endpoint.
  name: EndpointArn
  type: string
- description: The name of the endpoint configuration.
  name: EndpointConfigName
  type: string
- description: The status of the endpoint.
  name: EndpointStatus
  type: string
- description: An array of production variants.
  name: ProductionVariants
  type: array
- description: A timestamp indicating when the endpoint was created.
  name: CreationTime
  type: string
- description: A timestamp indicating when the endpoint was last modified.
  name: LastModifiedTime
  type: string
- description: If the status is Failed, the reason it failed.
  name: FailureReason
  type: string
provider_name: Amazon SageMaker
provider_slug: amazon-sagemaker
schema_file: json-schema/amazon-sagemaker-endpoint-schema.json
slug: amazon-sagemaker-endpoint
source_filename: amazon-sagemaker-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-sagemaker/refs/heads/main/json-schema/amazon-sagemaker-endpoint-schema.json\",\n  \"title\": \"Endpoint\",\n  \"description\": \"Endpoint schema from Amazon SageMaker API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the endpoint.\"\n    },\n    \"EndpointArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the endpoint.\"\n    },\n    \"EndpointConfigName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the endpoint configuration.\"\n    },\n    \"EndpointStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the endpoint.\",\n      \"enum\": [\n        \"OutOfService\",\n        \"Creating\",\n        \"Updating\",\n        \"SystemUpdating\",\n     \
  \   \"RollingBack\",\n        \"InService\",\n        \"Deleting\",\n        \"Failed\"\n      ]\n    },\n    \"ProductionVariants\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"VariantName\": {\n            \"type\": \"string\"\n          },\n          \"DeployedImages\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"SpecifiedImage\": {\n                  \"type\": \"string\"\n                },\n                \"ResolvedImage\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          },\n          \"CurrentWeight\": {\n            \"type\": \"number\"\n          },\n          \"DesiredWeight\": {\n            \"type\": \"number\"\n          },\n          \"CurrentInstanceCount\": {\n            \"type\": \"integer\"\n          },\n          \"DesiredInstanceCount\"\
  : {\n            \"type\": \"integer\"\n          }\n        }\n      },\n      \"description\": \"An array of production variants.\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"A timestamp indicating when the endpoint was created.\"\n    },\n    \"LastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"A timestamp indicating when the endpoint was last modified.\"\n    },\n    \"FailureReason\": {\n      \"type\": \"string\",\n      \"description\": \"If the status is Failed, the reason it failed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-sagemaker/refs/heads/main/json-schema/amazon-sagemaker-endpoint-schema.json
tags:
- AI
- AWS
- Inference
- Machine Learning
- MLOps
- Training
title: Endpoint
---
