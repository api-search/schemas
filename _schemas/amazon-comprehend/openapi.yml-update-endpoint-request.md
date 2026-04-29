---
description: UpdateEndpointRequest schema
layout: schema
name: UpdateEndpointRequest
properties_list:
- description: ''
  name: EndpointArn
  type: object
- description: ''
  name: DesiredModelArn
  type: object
- description: ''
  name: DesiredInferenceUnits
  type: object
- description: ''
  name: DesiredDataAccessRoleArn
  type: object
- description: ''
  name: FlywheelArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-update-endpoint-request-schema.json
slug: openapi.yml-update-endpoint-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-update-endpoint-request-schema.json\",\n  \"title\": \"UpdateEndpointRequest\",\n  \"description\": \"UpdateEndpointRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendEndpointArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the endpoint being updated.\"\n        }\n      ]\n    },\n    \"DesiredModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"The ARN of the new model to use when updating an existing endpoint.\"\n        }\n      ]\n    },\n    \"DesiredInferenceUnits\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/InferenceUnitsInteger\"\n        },\n        {\n          \"description\": \" The desired number of inference units to be used by the model using this endpoint. Each inference unit represents of a throughput of 100 characters per second.\"\n        }\n      ]\n    },\n    \"DesiredDataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"Data access role ARN to use in case the new model is encrypted with a customer CMK.\"\n        }\n      ]\n    },\n    \"FlywheelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendFlywheelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the flywheel\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-update-endpoint-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: UpdateEndpointRequest
---
