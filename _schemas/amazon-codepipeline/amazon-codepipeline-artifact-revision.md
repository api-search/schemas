---
description: Represents revision details of an artifact.
layout: schema
name: ArtifactRevision
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: revisionId
  type: object
- description: ''
  name: revisionChangeIdentifier
  type: object
- description: ''
  name: revisionSummary
  type: object
- description: ''
  name: created
  type: object
- description: ''
  name: revisionUrl
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-artifact-revision-schema.json
slug: amazon-codepipeline-artifact-revision
source_filename: amazon-codepipeline-artifact-revision-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-artifact-revision-schema.json\",\n  \"title\": \"ArtifactRevision\",\n  \"description\": \"Represents revision details of an artifact. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactName\"\n        },\n        {\n          \"description\": \"The name of an artifact. This name might be system-generated, such as \\\"MyApp\\\", or defined by the user when an action is created.\"\n        }\n      ]\n    },\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Revision\"\n        },\n        {\n          \"description\": \"The revision ID of the artifact.\"\n        }\n      ]\n    },\n    \"revisionChangeIdentifier\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/RevisionChangeIdentifier\"\n        },\n        {\n          \"description\": \"An additional identifier for a revision, such as a commit date or, for artifacts stored in Amazon S3 buckets, the ETag value.\"\n        }\n      ]\n    },\n    \"revisionSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionSummary\"\n        },\n        {\n          \"description\": \"Summary information about the most recent revision of the artifact. For GitHub and CodeCommit repositories, the commit message. For Amazon S3 buckets or actions, the user-provided content of a <code>codepipeline-artifact-revision-summary</code> key specified in the object metadata.\"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the most recent revision of the artifact\
  \ was created, in timestamp format.\"\n        }\n      ]\n    },\n    \"revisionUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Url\"\n        },\n        {\n          \"description\": \"The commit ID for the artifact revision. For artifacts stored in GitHub or CodeCommit repositories, the commit ID is linked to a commit details page.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-artifact-revision-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ArtifactRevision
---
