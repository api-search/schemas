---
description: Represents information about a current revision.
layout: schema
name: CurrentRevision
properties_list:
- description: ''
  name: revision
  type: object
- description: ''
  name: changeIdentifier
  type: object
- description: ''
  name: created
  type: object
- description: ''
  name: revisionSummary
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-current-revision-schema.json
slug: amazon-codepipeline-current-revision
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-current-revision-schema.json\",\n  \"title\": \"CurrentRevision\",\n  \"description\": \"Represents information about a current revision.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Revision\"\n        },\n        {\n          \"description\": \"The revision ID of the current version of an artifact.\"\n        }\n      ]\n    },\n    \"changeIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionChangeIdentifier\"\n        },\n        {\n          \"description\": \"The change identifier for the current revision.\"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\
  \n        },\n        {\n          \"description\": \"The date and time when the most recent revision of the artifact was created, in timestamp format.\"\n        }\n      ]\n    },\n    \"revisionSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionSummary\"\n        },\n        {\n          \"description\": \"The summary of the most recent revision of the artifact.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"revision\",\n    \"changeIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-current-revision-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: CurrentRevision
---
