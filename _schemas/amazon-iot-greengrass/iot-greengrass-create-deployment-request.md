---
description: CreateDeploymentRequest schema
layout: schema
name: CreateDeploymentRequest
properties_list:
- description: ''
  name: targetArn
  type: object
- description: ''
  name: deploymentName
  type: object
- description: ''
  name: components
  type: object
- description: ''
  name: iotJobConfiguration
  type: object
- description: ''
  name: deploymentPolicies
  type: object
- description: ''
  name: parentTargetArn
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-create-deployment-request-schema.json
slug: iot-greengrass-create-deployment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-create-deployment-request-schema.json\",\n  \"title\": \"CreateDeploymentRequest\",\n  \"description\": \"CreateDeploymentRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the target IoT thing or thing group. When creating a subdeployment, the targetARN can only be a thing group.\"\n        }\n      ]\n    },\n    \"deploymentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentNameString\"\n        },\n        {\n          \"description\": \"The name of the deployment.\"\
  \n        }\n      ]\n    },\n    \"components\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentDeploymentSpecifications\"\n        },\n        {\n          \"description\": \"The components to deploy. This is a dictionary, where each key is the name of a component, and each key's value is the version and configuration to deploy for that component.\"\n        }\n      ]\n    },\n    \"iotJobConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentIoTJobConfiguration\"\n        },\n        {\n          \"description\": \"The job configuration for the deployment configuration. The job configuration specifies the rollout, timeout, and stop configurations for the deployment configuration.\"\n        }\n      ]\n    },\n    \"deploymentPolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentPolicies\"\n        },\n        {\n          \"description\": \"The deployment\
  \ policies for the deployment. These policies define how the deployment updates components and handles failure.\"\n        }\n      ]\n    },\n    \"parentTargetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupARN\"\n        },\n        {\n          \"description\": \"The parent deployment's target <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> within a subdeployment.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A list of key-value pairs that contain metadata for the resource. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/tag-resources.html\\\">Tag your resources</a> in the <i>IoT Greengrass V2 Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/ClientTokenString\"\n        },\n        {\n          \"description\": \"A unique, case-sensitive identifier that you can provide to ensure that the request is idempotent. Idempotency means that the request is successfully processed only once, even if you send the request multiple times. When a request succeeds, and you specify the same client token for subsequent successful requests, the IoT Greengrass V2 service returns the successful response that it caches from the previous request. IoT Greengrass V2 caches successful responses for idempotent requests for up to 8 hours.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"targetArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-create-deployment-request-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: CreateDeploymentRequest
---
