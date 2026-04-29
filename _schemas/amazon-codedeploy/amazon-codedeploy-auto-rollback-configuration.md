---
description: Information about a configuration for automatically rolling back to a previous version of an application revision when a deployment is not completed successfully.
layout: schema
name: AutoRollbackConfiguration
properties_list:
- description: ''
  name: enabled
  type: object
- description: ''
  name: events
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-auto-rollback-configuration-schema.json
slug: amazon-codedeploy-auto-rollback-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-auto-rollback-configuration-schema.json\",\n  \"title\": \"AutoRollbackConfiguration\",\n  \"description\": \"Information about a configuration for automatically rolling back to a previous version of an application revision when a deployment is not completed successfully.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether a defined automatic rollback configuration is currently enabled.\"\n        }\n      ]\n    },\n    \"events\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoRollbackEventsList\"\n        },\n        {\n          \"description\": \"The event type or types that\
  \ trigger a rollback.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-auto-rollback-configuration-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: AutoRollbackConfiguration
---
