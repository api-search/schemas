---
description: Information about a deployment rollback.
layout: schema
name: RollbackInfo
properties_list:
- description: ''
  name: rollbackDeploymentId
  type: object
- description: ''
  name: rollbackTriggeringDeploymentId
  type: object
- description: ''
  name: rollbackMessage
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-rollback-info-schema.json
slug: amazon-codedeploy-rollback-info
source_filename: amazon-codedeploy-rollback-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-rollback-info-schema.json\",\n  \"title\": \"RollbackInfo\",\n  \"description\": \"Information about a deployment rollback.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rollbackDeploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \"The ID of the deployment rollback.\"\n        }\n      ]\n    },\n    \"rollbackTriggeringDeploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \"The deployment ID of the deployment that was underway and triggered a rollback deployment because it failed or was stopped.\"\n        }\n      ]\n    },\n    \"rollbackMessage\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"Information that describes the status of a deployment rollback (for example, whether the deployment can't be rolled back, is in progress, failed, or succeeded). \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-rollback-info-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: RollbackInfo
---
