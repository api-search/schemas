---
description: Represents an AWS CodeDeploy deployment with its configuration, status, and rollback settings.
layout: schema
name: Amazon CodeDeploy Deployment
properties_list:
- description: The unique ID of the deployment.
  name: deploymentId
  type: string
- description: The application name.
  name: applicationName
  type: string
- description: The deployment group name.
  name: deploymentGroupName
  type: string
- description: The current state of the deployment.
  name: status
  type: string
- description: The destination platform type for the deployment.
  name: computePlatform
  type: string
- description: Information about the location of stored application artifacts.
  name: revision
  type: object
- description: A comment about the deployment.
  name: description
  type: string
- description: The means by which the deployment was created.
  name: creator
  type: string
- description: A timestamp that indicates when the deployment was created.
  name: createTime
  type: string
- description: A timestamp that indicates when the deployment was deployed to the deployment group.
  name: startTime
  type: string
- description: A timestamp that indicates when the deployment was complete.
  name: completeTime
  type: string
- description: Information about the automatic rollback configuration.
  name: autoRollbackConfiguration
  type: object
- description: Information about a deployment rollback.
  name: rollbackInfo
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-deployment-schema.json
slug: amazon-codedeploy-deployment
source_filename: amazon-codedeploy-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/codedeploy/deployment.json\",\n  \"title\": \"Amazon CodeDeploy Deployment\",\n  \"description\": \"Represents an AWS CodeDeploy deployment with its configuration, status, and rollback settings.\",\n  \"type\": \"object\",\n  \"required\": [\"deploymentId\"],\n  \"properties\": {\n    \"deploymentId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the deployment.\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"The application name.\"\n    },\n    \"deploymentGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"The deployment group name.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the deployment.\",\n      \"enum\": [\n        \"Created\",\n        \"Queued\",\n        \"InProgress\",\n        \"Baking\"\
  ,\n        \"Succeeded\",\n        \"Failed\",\n        \"Stopped\",\n        \"Ready\"\n      ]\n    },\n    \"computePlatform\": {\n      \"type\": \"string\",\n      \"description\": \"The destination platform type for the deployment.\",\n      \"enum\": [\"Server\", \"Lambda\", \"ECS\"]\n    },\n    \"revision\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the location of stored application artifacts.\",\n      \"properties\": {\n        \"revisionType\": {\n          \"type\": \"string\",\n          \"enum\": [\"S3\", \"GitHub\", \"String\", \"AppSpecContent\"]\n        },\n        \"s3Location\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"bucket\": {\n              \"type\": \"string\"\n            },\n            \"key\": {\n              \"type\": \"string\"\n            },\n            \"bundleType\": {\n              \"type\": \"string\",\n              \"enum\": [\"tar\", \"tgz\", \"zip\", \"YAML\", \"JSON\"\
  ]\n            },\n            \"version\": {\n              \"type\": \"string\"\n            },\n            \"eTag\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"gitHubLocation\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"repository\": {\n              \"type\": \"string\"\n            },\n            \"commitId\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A comment about the deployment.\",\n      \"maxLength\": 256\n    },\n    \"creator\": {\n      \"type\": \"string\",\n      \"description\": \"The means by which the deployment was created.\",\n      \"enum\": [\"user\", \"autoscaling\", \"codeDeployRollback\", \"CodeDeploy\", \"CodeDeployAutoUpdate\"]\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"\
  A timestamp that indicates when the deployment was created.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"A timestamp that indicates when the deployment was deployed to the deployment group.\"\n    },\n    \"completeTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"A timestamp that indicates when the deployment was complete.\"\n    },\n    \"autoRollbackConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the automatic rollback configuration.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\"\n        },\n        \"events\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"DEPLOYMENT_FAILURE\",\n              \"DEPLOYMENT_STOP_ON_ALARM\",\n              \"DEPLOYMENT_STOP_ON_REQUEST\"\n            ]\n       \
  \   }\n        }\n      }\n    },\n    \"rollbackInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Information about a deployment rollback.\",\n      \"properties\": {\n        \"rollbackDeploymentId\": {\n          \"type\": \"string\"\n        },\n        \"rollbackTriggeringDeploymentId\": {\n          \"type\": \"string\"\n        },\n        \"rollbackMessage\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: Amazon CodeDeploy Deployment
---
