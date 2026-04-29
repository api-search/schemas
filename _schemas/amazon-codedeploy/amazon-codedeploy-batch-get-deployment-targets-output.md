---
description: BatchGetDeploymentTargetsOutput schema from Amazon CodeDeploy
layout: schema
name: BatchGetDeploymentTargetsOutput
properties_list:
- description: ''
  name: deploymentTargets
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-batch-get-deployment-targets-output-schema.json
slug: amazon-codedeploy-batch-get-deployment-targets-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployment-targets-output-schema.json\",\n  \"title\": \"BatchGetDeploymentTargetsOutput\",\n  \"description\": \"BatchGetDeploymentTargetsOutput schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentTargets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentTargetList\"\n        },\n        {\n          \"description\": \"<p> A list of target objects for a deployment. Each target object contains details about the target, such as its status and lifecycle events. The type of the target objects depends on the deployment' compute platform. </p> <ul> <li> <p> <b>EC2/On-premises</b>: Each target object is an Amazon EC2 or on-premises instance. </p> </li> <li> <p> <b>Lambda</b>: The target object is\
  \ a specific version of an Lambda function. </p> </li> <li> <p> <b>Amazon ECS</b>: The target object is an Amazon ECS service. </p> </li> <li> <p> <b>CloudFormation</b>: The target object is an CloudFormation blue/green deployment. </p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-deployment-targets-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BatchGetDeploymentTargetsOutput
---
