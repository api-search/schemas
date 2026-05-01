---
description: PutLifecycleEventHookExecutionStatusOutput schema from Amazon CodeDeploy
layout: schema
name: PutLifecycleEventHookExecutionStatusOutput
properties_list:
- description: ''
  name: lifecycleEventHookExecutionId
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-put-lifecycle-event-hook-execution-status-output-schema.json
slug: amazon-codedeploy-put-lifecycle-event-hook-execution-status-output
source_filename: amazon-codedeploy-put-lifecycle-event-hook-execution-status-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-put-lifecycle-event-hook-execution-status-output-schema.json\",\n  \"title\": \"PutLifecycleEventHookExecutionStatusOutput\",\n  \"description\": \"PutLifecycleEventHookExecutionStatusOutput schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lifecycleEventHookExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleEventHookExecutionId\"\n        },\n        {\n          \"description\": \"The execution ID of the lifecycle event hook. A hook is specified in the <code>hooks</code> section of the deployment's AppSpec file.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-put-lifecycle-event-hook-execution-status-output-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: PutLifecycleEventHookExecutionStatusOutput
---
