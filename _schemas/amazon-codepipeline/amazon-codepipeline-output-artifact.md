---
description: Represents information about the output of an action.
layout: schema
name: OutputArtifact
properties_list:
- description: ''
  name: name
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-output-artifact-schema.json
slug: amazon-codepipeline-output-artifact
source_filename: amazon-codepipeline-output-artifact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-output-artifact-schema.json\",\n  \"title\": \"OutputArtifact\",\n  \"description\": \"Represents information about the output of an action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactName\"\n        },\n        {\n          \"description\": \"<p>The name of the output of an artifact, such as \\\"My App\\\".</p> <p>The input artifact of an action must exactly match the output artifact declared in a preceding action, but the input artifact does not have to be the next action in strict sequence from the action that provided the output artifact. Actions in parallel can declare different output artifacts, which are in turn consumed by different following actions.</p> <p>Output artifact\
  \ names must be unique within a pipeline.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-output-artifact-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: OutputArtifact
---
