---
description: Information about the deployment status of the instances in the deployment.
layout: schema
name: DeploymentOverview
properties_list:
- description: ''
  name: Pending
  type: object
- description: ''
  name: InProgress
  type: object
- description: ''
  name: Succeeded
  type: object
- description: ''
  name: Failed
  type: object
- description: ''
  name: Skipped
  type: object
- description: ''
  name: Ready
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-deployment-overview-schema.json
slug: amazon-codedeploy-deployment-overview
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-overview-schema.json\",\n  \"title\": \"DeploymentOverview\",\n  \"description\": \"Information about the deployment status of the instances in the deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Pending\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceCount\"\n        },\n        {\n          \"description\": \"The number of instances in the deployment in a pending state.\"\n        }\n      ]\n    },\n    \"InProgress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceCount\"\n        },\n        {\n          \"description\": \"The number of instances in which the deployment is in progress.\"\n        }\n      ]\n    },\n    \"Succeeded\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/InstanceCount\"\n        },\n        {\n          \"description\": \"The number of instances in the deployment to which revisions have been successfully deployed.\"\n        }\n      ]\n    },\n    \"Failed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceCount\"\n        },\n        {\n          \"description\": \"The number of instances in the deployment in a failed state.\"\n        }\n      ]\n    },\n    \"Skipped\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceCount\"\n        },\n        {\n          \"description\": \"The number of instances in the deployment in a skipped state.\"\n        }\n      ]\n    },\n    \"Ready\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceCount\"\n        },\n        {\n          \"description\": \"The number of instances in a replacement environment ready to receive traffic in a blue/green\
  \ deployment.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deployment-overview-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: DeploymentOverview
---
