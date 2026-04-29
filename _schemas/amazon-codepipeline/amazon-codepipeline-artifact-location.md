---
description: Represents information about the location of an artifact.
layout: schema
name: ArtifactLocation
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: s3Location
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-artifact-location-schema.json
slug: amazon-codepipeline-artifact-location
source_filename: amazon-codepipeline-artifact-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-artifact-location-schema.json\",\n  \"title\": \"ArtifactLocation\",\n  \"description\": \"Represents information about the location of an artifact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactLocationType\"\n        },\n        {\n          \"description\": \"The type of artifact in the location.\"\n        }\n      ]\n    },\n    \"s3Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ArtifactLocation\"\n        },\n        {\n          \"description\": \"The S3 bucket that contains the artifact.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-artifact-location-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ArtifactLocation
---
