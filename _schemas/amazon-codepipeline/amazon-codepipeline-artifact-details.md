---
description: Returns information about the details of an artifact.
layout: schema
name: ArtifactDetails
properties_list:
- description: ''
  name: minimumCount
  type: object
- description: ''
  name: maximumCount
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-artifact-details-schema.json
slug: amazon-codepipeline-artifact-details
source_filename: amazon-codepipeline-artifact-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-artifact-details-schema.json\",\n  \"title\": \"ArtifactDetails\",\n  \"description\": \"Returns information about the details of an artifact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"minimumCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinimumArtifactCount\"\n        },\n        {\n          \"description\": \"The minimum number of artifacts allowed for the action type.\"\n        }\n      ]\n    },\n    \"maximumCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumArtifactCount\"\n        },\n        {\n          \"description\": \"The maximum number of artifacts allowed for the action type.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"minimumCount\",\n    \"maximumCount\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-artifact-details-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ArtifactDetails
---
