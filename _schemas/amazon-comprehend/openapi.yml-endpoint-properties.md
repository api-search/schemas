---
description: Specifies information about the specified endpoint. For information about endpoints, see <a href="https://docs.aws.amazon.com/comprehend/latest/dg/manage-endpoints.html">Managing endpoints</a>.
layout: schema
name: EndpointProperties
properties_list:
- description: ''
  name: EndpointArn
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Message
  type: object
- description: ''
  name: ModelArn
  type: object
- description: ''
  name: DesiredModelArn
  type: object
- description: ''
  name: DesiredInferenceUnits
  type: object
- description: ''
  name: CurrentInferenceUnits
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: LastModifiedTime
  type: object
- description: ''
  name: DataAccessRoleArn
  type: object
- description: ''
  name: DesiredDataAccessRoleArn
  type: object
- description: ''
  name: FlywheelArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-endpoint-properties-schema.json
slug: openapi.yml-endpoint-properties
source_filename: openapi.yml-endpoint-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-endpoint-properties-schema.json\",\n  \"title\": \"EndpointProperties\",\n  \"description\": \"Specifies information about the specified endpoint. For information about endpoints, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/manage-endpoints.html\\\">Managing endpoints</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendEndpointArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the endpoint.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointStatus\"\n        },\n        {\n          \"description\": \"Specifies the status of the endpoint.\
  \ Because the endpoint updates and creation are asynchronous, so customers will need to wait for the endpoint to be <code>Ready</code> status before making inference requests.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnyLengthString\"\n        },\n        {\n          \"description\": \"Specifies a reason for failure in cases of <code>Failed</code> status.\"\n        }\n      ]\n    },\n    \"ModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the model to which the endpoint is attached.\"\n        }\n      ]\n    },\n    \"DesiredModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"ARN of the new model to use for updating an existing endpoint. This ARN\
  \ is going to be different from the model ARN when the update is in progress\"\n        }\n      ]\n    },\n    \"DesiredInferenceUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InferenceUnitsInteger\"\n        },\n        {\n          \"description\": \"The desired number of inference units to be used by the model using this endpoint. Each inference unit represents of a throughput of 100 characters per second.\"\n        }\n      ]\n    },\n    \"CurrentInferenceUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InferenceUnitsInteger\"\n        },\n        {\n          \"description\": \"The number of inference units currently used by the model using this endpoint.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The creation date and time of the endpoint.\"\n        }\n\
  \      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time that the endpoint was last modified.\"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that grants Amazon Comprehend read access to trained custom models encrypted with a customer managed key (ModelKmsKeyId).\"\n        }\n      ]\n    },\n    \"DesiredDataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"Data access role ARN to use in case the new model is encrypted with a customer KMS key.\"\n        }\n      ]\n    },\n    \"FlywheelArn\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/ComprehendFlywheelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the flywheel\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-endpoint-properties-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EndpointProperties
---
