---
description: GetDeploymentResponse schema
layout: schema
name: GetDeploymentResponse
properties_list:
- description: ''
  name: targetArn
  type: object
- description: ''
  name: revisionId
  type: object
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: deploymentName
  type: object
- description: ''
  name: deploymentStatus
  type: object
- description: ''
  name: iotJobId
  type: object
- description: ''
  name: iotJobArn
  type: object
- description: ''
  name: components
  type: object
- description: ''
  name: deploymentPolicies
  type: object
- description: ''
  name: iotJobConfiguration
  type: object
- description: ''
  name: creationTimestamp
  type: object
- description: ''
  name: isLatestForTarget
  type: object
- description: ''
  name: parentTargetArn
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-get-deployment-response-schema.json
slug: iot-greengrass-get-deployment-response
source_filename: iot-greengrass-get-deployment-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-get-deployment-response-schema.json\",\n  \"title\": \"GetDeploymentResponse\",\n  \"description\": \"GetDeploymentResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the target IoT thing or thing group.\"\n        }\n      ]\n    },\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The revision number of the deployment.\"\n        }\n      ]\n    },\n    \"deploymentId\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ID of the deployment.\"\n        }\n      ]\n    },\n    \"deploymentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableString\"\n        },\n        {\n          \"description\": \"The name of the deployment.\"\n        }\n      ]\n    },\n    \"deploymentStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStatus\"\n        },\n        {\n          \"description\": \"The status of the deployment.\"\n        }\n      ]\n    },\n    \"iotJobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableString\"\n        },\n        {\n          \"description\": \"The ID of the IoT job that applies the deployment to target devices.\"\n        }\n      ]\n    },\n    \"iotJobArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobARN\"\
  \n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the IoT job that applies the deployment to target devices.\"\n        }\n      ]\n    },\n    \"components\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentDeploymentSpecifications\"\n        },\n        {\n          \"description\": \"The components to deploy. This is a dictionary, where each key is the name of a component, and each key's value is the version and configuration to deploy for that component.\"\n        }\n      ]\n    },\n    \"deploymentPolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentPolicies\"\n        },\n        {\n          \"description\": \"The deployment policies for the deployment. These policies define how the deployment updates components and handles failure.\"\n        }\n      ]\n    },\n    \"iotJobConfiguration\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentIoTJobConfiguration\"\n        },\n        {\n          \"description\": \"The job configuration for the deployment configuration. The job configuration specifies the rollout, timeout, and stop configurations for the deployment configuration.\"\n        }\n      ]\n    },\n    \"creationTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the deployment was created, expressed in ISO 8601 format.\"\n        }\n      ]\n    },\n    \"isLatestForTarget\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IsLatestForTarget\"\n        },\n        {\n          \"description\": \"Whether or not the deployment is the latest revision for its target.\"\n        }\n      ]\n    },\n    \"parentTargetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupARN\"\
  \n        },\n        {\n          \"description\": \"The parent deployment's target <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> within a subdeployment.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A list of key-value pairs that contain metadata for the resource. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/tag-resources.html\\\">Tag your resources</a> in the <i>IoT Greengrass V2 Developer Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-get-deployment-response-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: GetDeploymentResponse
---
