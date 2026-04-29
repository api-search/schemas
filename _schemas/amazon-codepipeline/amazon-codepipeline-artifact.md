---
description: 'Artifacts are the files that are worked on by actions in the pipeline. See the action configuration for each action for details about artifact parameters. For example, the S3 source action artifact is a file name (or file path), and the files are generally provided as a ZIP file. Example artifact name: SampleApp_Windows.zip'
layout: schema
name: Artifact
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: revision
  type: object
- description: ''
  name: location
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-artifact-schema.json
slug: amazon-codepipeline-artifact
source_filename: amazon-codepipeline-artifact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-artifact-schema.json\",\n  \"title\": \"Artifact\",\n  \"description\": \"Artifacts are the files that are worked on by actions in the pipeline. See the action configuration for each action for details about artifact parameters. For example, the S3 source action artifact is a file name (or file path), and the files are generally provided as a ZIP file. Example artifact name: SampleApp_Windows.zip\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactName\"\n        },\n        {\n          \"description\": \"The artifact's name.\"\n        }\n      ]\n    },\n    \"revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Revision\"\n        },\n        {\n\
  \          \"description\": \"The artifact's revision ID. Depending on the type of object, this could be a commit ID (GitHub) or a revision ID (Amazon S3).\"\n        }\n      ]\n    },\n    \"location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactLocation\"\n        },\n        {\n          \"description\": \"The location of an artifact.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-artifact-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: Artifact
---
