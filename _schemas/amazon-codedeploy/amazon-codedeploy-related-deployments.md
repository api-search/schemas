---
description: Information about deployments related to the specified deployment.
layout: schema
name: RelatedDeployments
properties_list:
- description: ''
  name: autoUpdateOutdatedInstancesRootDeploymentId
  type: object
- description: ''
  name: autoUpdateOutdatedInstancesDeploymentIds
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-related-deployments-schema.json
slug: amazon-codedeploy-related-deployments
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-related-deployments-schema.json\",\n  \"title\": \"RelatedDeployments\",\n  \"description\": \"Information about deployments related to the specified deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"autoUpdateOutdatedInstancesRootDeploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \"The deployment ID of the root deployment that triggered this deployment.\"\n        }\n      ]\n    },\n    \"autoUpdateOutdatedInstancesDeploymentIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentsList\"\n        },\n        {\n          \"description\": \"The deployment IDs of 'auto-update outdated instances' deployments triggered by this\
  \ deployment.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-related-deployments-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: RelatedDeployments
---
