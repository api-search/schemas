---
description: Information about whether instances in the original environment are terminated when a blue/green deployment is successful. <code>BlueInstanceTerminationOption</code> does not apply to Lambda deployments.
layout: schema
name: BlueInstanceTerminationOption
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: terminationWaitTimeInMinutes
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-blue-instance-termination-option-schema.json
slug: amazon-codedeploy-blue-instance-termination-option
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-blue-instance-termination-option-schema.json\",\n  \"title\": \"BlueInstanceTerminationOption\",\n  \"description\": \"Information about whether instances in the original environment are terminated when a blue/green deployment is successful. <code>BlueInstanceTerminationOption</code> does not apply to Lambda deployments. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceAction\"\n        },\n        {\n          \"description\": \"<p>The action to take on instances in the original environment after a successful blue/green deployment.</p> <ul> <li> <p> <code>TERMINATE</code>: Instances are terminated after a specified wait time.</p> </li> <li> <p> <code>KEEP_ALIVE</code>: Instances are\
  \ left running after they are deregistered from the load balancer and removed from the deployment group.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"terminationWaitTimeInMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Duration\"\n        },\n        {\n          \"description\": \"<p>For an Amazon EC2 deployment, the number of minutes to wait after a successful blue/green deployment before terminating instances from the original environment.</p> <p> For an Amazon ECS deployment, the number of minutes before deleting the original (blue) task set. During an Amazon ECS deployment, CodeDeploy shifts traffic from the original (blue) task set to a replacement (green) task set. </p> <p> The maximum setting is 2880 minutes (2 days). </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-blue-instance-termination-option-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BlueInstanceTerminationOption
---
