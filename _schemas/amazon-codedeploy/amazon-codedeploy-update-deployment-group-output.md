---
description: Represents the output of an <code>UpdateDeploymentGroup</code> operation.
layout: schema
name: UpdateDeploymentGroupOutput
properties_list:
- description: ''
  name: hooksNotCleanedUp
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-update-deployment-group-output-schema.json
slug: amazon-codedeploy-update-deployment-group-output
source_filename: amazon-codedeploy-update-deployment-group-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-update-deployment-group-output-schema.json\",\n  \"title\": \"UpdateDeploymentGroupOutput\",\n  \"description\": \"Represents the output of an <code>UpdateDeploymentGroup</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hooksNotCleanedUp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupList\"\n        },\n        {\n          \"description\": \"If the output contains no data, and the corresponding deployment group contained at least one Auto Scaling group, CodeDeploy successfully removed all corresponding Auto Scaling lifecycle event hooks from the Amazon Web Services account. If the output contains data, CodeDeploy could not remove some Auto Scaling lifecycle event hooks from the Amazon Web Services account.\"\n\
  \        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-update-deployment-group-output-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: UpdateDeploymentGroupOutput
---
