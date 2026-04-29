---
description: BatchGetDeploymentTargetsInput schema from Amazon CodeDeploy
layout: schema
name: BatchGetDeploymentTargetsInput
properties_list:
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: targetIds
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-batch-get-deployment-targets-input-schema.json
slug: amazon-codedeploy-batch-get-deployment-targets-input
source_filename: amazon-codedeploy-batch-get-deployment-targets-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployment-targets-input-schema.json\",\n  \"title\": \"BatchGetDeploymentTargetsInput\",\n  \"description\": \"BatchGetDeploymentTargetsInput schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment. \"\n        }\n      ]\n    },\n    \"targetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetIdList\"\n        },\n        {\n          \"description\": \"<p> The unique IDs of the deployment targets. The compute platform of the deployment determines the type of the targets and their formats. The maximum number of deployment\
  \ target IDs you can specify is 25.</p> <ul> <li> <p> For deployments that use the EC2/On-premises compute platform, the target IDs are Amazon EC2 or on-premises instances IDs, and their target type is <code>instanceTarget</code>. </p> </li> <li> <p> For deployments that use the Lambda compute platform, the target IDs are the names of Lambda functions, and their target type is <code>instanceTarget</code>. </p> </li> <li> <p> For deployments that use the Amazon ECS compute platform, the target IDs are pairs of Amazon ECS clusters and services specified using the format <code>&lt;clustername&gt;:&lt;servicename&gt;</code>. Their target type is <code>ecsTarget</code>. </p> </li> <li> <p> For deployments that are deployed with CloudFormation, the target IDs are CloudFormation stack IDs. Their target type is <code>cloudFormationTarget</code>. </p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployment-targets-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BatchGetDeploymentTargetsInput
---
