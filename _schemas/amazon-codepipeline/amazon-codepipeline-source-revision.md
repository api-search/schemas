---
description: Information about the version (or revision) of a source artifact that initiated a pipeline execution.
layout: schema
name: SourceRevision
properties_list:
- description: ''
  name: actionName
  type: object
- description: ''
  name: revisionId
  type: object
- description: ''
  name: revisionSummary
  type: object
- description: ''
  name: revisionUrl
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-source-revision-schema.json
slug: amazon-codepipeline-source-revision
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-source-revision-schema.json\",\n  \"title\": \"SourceRevision\",\n  \"description\": \"Information about the version (or revision) of a source artifact that initiated a pipeline execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionName\"\n        },\n        {\n          \"description\": \"The name of the action that processed the revision to the source artifact.\"\n        }\n      ]\n    },\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Revision\"\n        },\n        {\n          \"description\": \"The system-generated unique ID that identifies the revision number of the artifact.\"\n        }\n      ]\n    },\n    \"\
  revisionSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionSummary\"\n        },\n        {\n          \"description\": \"Summary information about the most recent revision of the artifact. For GitHub and CodeCommit repositories, the commit message. For Amazon S3 buckets or actions, the user-provided content of a <code>codepipeline-artifact-revision-summary</code> key specified in the object metadata.\"\n        }\n      ]\n    },\n    \"revisionUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Url\"\n        },\n        {\n          \"description\": \"The commit ID for the artifact revision. For artifacts stored in GitHub or CodeCommit repositories, the commit ID is linked to a commit details page.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"actionName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-source-revision-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: SourceRevision
---
