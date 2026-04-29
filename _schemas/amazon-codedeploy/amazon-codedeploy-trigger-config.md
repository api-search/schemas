---
description: Information about notification triggers for the deployment group.
layout: schema
name: TriggerConfig
properties_list:
- description: ''
  name: triggerName
  type: object
- description: ''
  name: triggerTargetArn
  type: object
- description: ''
  name: triggerEvents
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-trigger-config-schema.json
slug: amazon-codedeploy-trigger-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-trigger-config-schema.json\",\n  \"title\": \"TriggerConfig\",\n  \"description\": \"Information about notification triggers for the deployment group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"triggerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerName\"\n        },\n        {\n          \"description\": \"The name of the notification trigger.\"\n        }\n      ]\n    },\n    \"triggerTargetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerTargetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Amazon Simple Notification Service topic through which notifications about deployment or instance events are sent.\"\n        }\n      ]\n    },\n\
  \    \"triggerEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerEventTypeList\"\n        },\n        {\n          \"description\": \"The event type or types for which notifications are triggered.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-trigger-config-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: TriggerConfig
---
