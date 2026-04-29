---
description: CreateEndpointRequest schema
layout: schema
name: CreateEndpointRequest
properties_list:
- description: ''
  name: EndpointName
  type: object
- description: ''
  name: ModelArn
  type: object
- description: ''
  name: DesiredInferenceUnits
  type: object
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: DataAccessRoleArn
  type: object
- description: ''
  name: FlywheelArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-create-endpoint-request-schema.json
slug: openapi.yml-create-endpoint-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-create-endpoint-request-schema.json\",\n  \"title\": \"CreateEndpointRequest\",\n  \"description\": \"CreateEndpointRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendEndpointName\"\n        },\n        {\n          \"description\": \"This is the descriptive suffix that becomes part of the <code>EndpointArn</code> used for all subsequent requests to this resource. \"\n        }\n      ]\n    },\n    \"ModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the model to which the endpoint will be attached.\"\n        }\n      ]\n\
  \    },\n    \"DesiredInferenceUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InferenceUnitsInteger\"\n        },\n        {\n          \"description\": \" The desired number of inference units to be used by the model using this endpoint. Each inference unit represents of a throughput of 100 characters per second.\"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestTokenString\"\n        },\n        {\n          \"description\": \"An idempotency token provided by the customer. If this token matches a previous endpoint creation request, Amazon Comprehend will not return a <code>ResourceInUseException</code>. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Tags to associate with the endpoint. A tag is a key-value pair\
  \ that adds metadata to the endpoint. For example, a tag with \\\"Sales\\\" as the key might be added to an endpoint to indicate its use by the sales department. \"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that grants Amazon Comprehend read access to trained custom models encrypted with a customer managed key (ModelKmsKeyId).\"\n        }\n      ]\n    },\n    \"FlywheelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendFlywheelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the flywheel to which the endpoint will be attached.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointName\",\n    \"DesiredInferenceUnits\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-create-endpoint-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: CreateEndpointRequest
---
