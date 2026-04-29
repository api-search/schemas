---
description: Information about an application revision.
layout: schema
name: GenericRevisionInfo
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: deploymentGroups
  type: object
- description: ''
  name: firstUsedTime
  type: object
- description: ''
  name: lastUsedTime
  type: object
- description: ''
  name: registerTime
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-generic-revision-info-schema.json
slug: amazon-codedeploy-generic-revision-info
source_filename: amazon-codedeploy-generic-revision-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-generic-revision-info-schema.json\",\n  \"title\": \"GenericRevisionInfo\",\n  \"description\": \"Information about an application revision.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A comment about the revision.\"\n        }\n      ]\n    },\n    \"deploymentGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentGroupsList\"\n        },\n        {\n          \"description\": \"The deployment groups for which this is the current target revision.\"\n        }\n      ]\n    },\n    \"firstUsedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"When the revision was first used by CodeDeploy.\"\n        }\n      ]\n    },\n    \"lastUsedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"When the revision was last used by CodeDeploy.\"\n        }\n      ]\n    },\n    \"registerTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"When the revision was registered with CodeDeploy.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-generic-revision-info-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GenericRevisionInfo
---
