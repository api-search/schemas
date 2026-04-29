---
description: Information about the deployment target.
layout: schema
name: DeploymentTarget
properties_list:
- description: ''
  name: deploymentTargetType
  type: object
- description: ''
  name: instanceTarget
  type: object
- description: ''
  name: lambdaTarget
  type: object
- description: ''
  name: ecsTarget
  type: object
- description: ''
  name: cloudFormationTarget
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-deployment-target-schema.json
slug: amazon-codedeploy-deployment-target
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-target-schema.json\",\n  \"title\": \"DeploymentTarget\",\n  \"description\": \" Information about the deployment target. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentTargetType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentTargetType\"\n        },\n        {\n          \"description\": \"The deployment type that is specific to the deployment's compute platform or deployments initiated by a CloudFormation stack update.\"\n        }\n      ]\n    },\n    \"instanceTarget\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceTarget\"\n        },\n        {\n          \"description\": \" Information about the target for a deployment that uses the EC2/On-premises compute platform.\
  \ \"\n        }\n      ]\n    },\n    \"lambdaTarget\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaTarget\"\n        },\n        {\n          \"description\": \" Information about the target for a deployment that uses the Lambda compute platform. \"\n        }\n      ]\n    },\n    \"ecsTarget\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSTarget\"\n        },\n        {\n          \"description\": \" Information about the target for a deployment that uses the Amazon ECS compute platform. \"\n        }\n      ]\n    },\n    \"cloudFormationTarget\": {\n      \"$ref\": \"#/components/schemas/CloudFormationTarget\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-target-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: DeploymentTarget
---
