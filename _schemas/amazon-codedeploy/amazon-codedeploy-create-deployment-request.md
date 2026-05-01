---
description: CreateDeploymentRequest schema from Amazon CodeDeploy
layout: schema
name: CreateDeploymentRequest
properties_list:
- description: The name of the application.
  name: applicationName
  type: string
- description: The name of the deployment group.
  name: deploymentGroupName
  type: string
- description: ''
  name: revision
  type: object
- description: A comment about the deployment.
  name: description
  type: string
- description: ''
  name: autoRollbackConfiguration
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-create-deployment-request-schema.json
slug: amazon-codedeploy-create-deployment-request
source_filename: amazon-codedeploy-create-deployment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-deployment-request-schema.json\",\n  \"title\": \"CreateDeploymentRequest\",\n  \"description\": \"CreateDeploymentRequest schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application.\"\n    },\n    \"deploymentGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the deployment group.\"\n    },\n    \"revision\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"revisionType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"S3\",\n            \"GitHub\",\n            \"String\",\n            \"AppSpecContent\"\n          ]\n        },\n        \"s3Location\": {\n          \"type\"\
  : \"object\",\n          \"properties\": {\n            \"bucket\": {\n              \"type\": \"string\"\n            },\n            \"key\": {\n              \"type\": \"string\"\n            },\n            \"bundleType\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"tar\",\n                \"tgz\",\n                \"zip\",\n                \"YAML\",\n                \"JSON\"\n              ]\n            }\n          }\n        },\n        \"gitHubLocation\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"repository\": {\n              \"type\": \"string\"\n            },\n            \"commitId\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A comment about the deployment.\"\n    },\n    \"autoRollbackConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n       \
  \ \"enabled\": {\n          \"type\": \"boolean\"\n        },\n        \"events\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"DEPLOYMENT_FAILURE\",\n              \"DEPLOYMENT_STOP_ON_ALARM\",\n              \"DEPLOYMENT_STOP_ON_REQUEST\"\n            ]\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"applicationName\",\n    \"deploymentGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-deployment-request-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: CreateDeploymentRequest
---
