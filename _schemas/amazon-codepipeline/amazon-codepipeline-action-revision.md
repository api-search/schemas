---
description: Represents information about the version (or revision) of an action.
layout: schema
name: ActionRevision
properties_list:
- description: ''
  name: revisionId
  type: object
- description: ''
  name: revisionChangeId
  type: object
- description: ''
  name: created
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-revision-schema.json
slug: amazon-codepipeline-action-revision
source_filename: amazon-codepipeline-action-revision-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-revision-schema.json\",\n  \"title\": \"ActionRevision\",\n  \"description\": \"Represents information about the version (or revision) of an action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Revision\"\n        },\n        {\n          \"description\": \"The system-generated unique ID that identifies the revision number of the action.\"\n        }\n      ]\n    },\n    \"revisionChangeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionChangeIdentifier\"\n        },\n        {\n          \"description\": \"The unique identifier of the change that set the state to this revision (for example, a deployment ID or timestamp).\"\n     \
  \   }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the most recent version of the action was created, in timestamp format.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"revisionId\",\n    \"revisionChangeId\",\n    \"created\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-revision-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionRevision
---
