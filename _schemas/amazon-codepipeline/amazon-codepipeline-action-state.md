---
description: Represents information about the state of an action.
layout: schema
name: ActionState
properties_list:
- description: ''
  name: actionName
  type: object
- description: ''
  name: currentRevision
  type: object
- description: ''
  name: latestExecution
  type: object
- description: ''
  name: entityUrl
  type: object
- description: ''
  name: revisionUrl
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-state-schema.json
slug: amazon-codepipeline-action-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-state-schema.json\",\n  \"title\": \"ActionState\",\n  \"description\": \"Represents information about the state of an action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionName\"\n        },\n        {\n          \"description\": \"The name of the action.\"\n        }\n      ]\n    },\n    \"currentRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionRevision\"\n        },\n        {\n          \"description\": \"Represents information about the version (or revision) of an action.\"\n        }\n      ]\n    },\n    \"latestExecution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionExecution\"\
  \n        },\n        {\n          \"description\": \"Represents information about the run of an action.\"\n        }\n      ]\n    },\n    \"entityUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Url\"\n        },\n        {\n          \"description\": \"A URL link for more information about the state of the action, such as a deployment group details page.\"\n        }\n      ]\n    },\n    \"revisionUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Url\"\n        },\n        {\n          \"description\": \"A URL link for more information about the revision, such as a commit details page.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-state-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionState
---
