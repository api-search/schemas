---
description: PutLifecycleEventHookExecutionStatusInput schema from Amazon CodeDeploy
layout: schema
name: PutLifecycleEventHookExecutionStatusInput
properties_list:
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: lifecycleEventHookExecutionId
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-put-lifecycle-event-hook-execution-status-input-schema.json
slug: amazon-codedeploy-put-lifecycle-event-hook-execution-status-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-put-lifecycle-event-hook-execution-status-input-schema.json\",\n  \"title\": \"PutLifecycleEventHookExecutionStatusInput\",\n  \"description\": \"PutLifecycleEventHookExecutionStatusInput schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \" The unique ID of a deployment. Pass this ID to a Lambda function that validates a deployment lifecycle event. \"\n        }\n      ]\n    },\n    \"lifecycleEventHookExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleEventHookExecutionId\"\n        },\n        {\n          \"description\": \" The execution\
  \ ID of a deployment's lifecycle hook. A deployment lifecycle hook is specified in the <code>hooks</code> section of the AppSpec file. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleEventStatus\"\n        },\n        {\n          \"description\": \"The result of a Lambda function that validates a deployment lifecycle event. The values listed in <b>Valid Values</b> are valid for lifecycle statuses in general; however, only <code>Succeeded</code> and <code>Failed</code> can be passed successfully in your API call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-put-lifecycle-event-hook-execution-status-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: PutLifecycleEventHookExecutionStatusInput
---
