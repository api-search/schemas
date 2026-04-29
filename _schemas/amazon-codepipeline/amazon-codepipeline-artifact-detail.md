---
description: Artifact details for the action execution, such as the artifact location.
layout: schema
name: ArtifactDetail
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: s3location
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-artifact-detail-schema.json
slug: amazon-codepipeline-artifact-detail
source_filename: amazon-codepipeline-artifact-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-artifact-detail-schema.json\",\n  \"title\": \"ArtifactDetail\",\n  \"description\": \"Artifact details for the action execution, such as the artifact location.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactName\"\n        },\n        {\n          \"description\": \"The artifact object name for the action execution.\"\n        }\n      ]\n    },\n    \"s3location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"The Amazon S3 artifact location for the action execution.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-artifact-detail-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ArtifactDetail
---
