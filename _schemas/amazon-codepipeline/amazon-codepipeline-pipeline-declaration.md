---
description: Represents the structure of actions and stages to be performed in the pipeline.
layout: schema
name: PipelineDeclaration
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: artifactStore
  type: object
- description: ''
  name: artifactStores
  type: object
- description: ''
  name: stages
  type: object
- description: ''
  name: version
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-pipeline-declaration-schema.json
slug: amazon-codepipeline-pipeline-declaration
source_filename: amazon-codepipeline-pipeline-declaration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-declaration-schema.json\",\n  \"title\": \"PipelineDeclaration\",\n  \"description\": \"Represents the structure of actions and stages to be performed in the pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for CodePipeline to use to either perform actions with no <code>actionRoleArn</code>, or to use to assume roles for actions with an <code>actionRoleArn</code>.\"\
  \n        }\n      ]\n    },\n    \"artifactStore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactStore\"\n        },\n        {\n          \"description\": \"<p>Represents information about the S3 bucket where artifacts are stored for the pipeline.</p> <note> <p>You must include either <code>artifactStore</code> or <code>artifactStores</code> in your pipeline, but you cannot use both. If you create a cross-region action in your pipeline, you must use <code>artifactStores</code>.</p> </note>\"\n        }\n      ]\n    },\n    \"artifactStores\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactStoreMap\"\n        },\n        {\n          \"description\": \"<p>A mapping of <code>artifactStore</code> objects and their corresponding Amazon Web Services Regions. There must be an artifact store for the pipeline Region and for each cross-region action in the pipeline.</p> <note> <p>You must include either <code>artifactStore</code>\
  \ or <code>artifactStores</code> in your pipeline, but you cannot use both. If you create a cross-region action in your pipeline, you must use <code>artifactStores</code>.</p> </note>\"\n        }\n      ]\n    },\n    \"stages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineStageDeclarationList\"\n        },\n        {\n          \"description\": \"The stage in which to perform the action.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineVersion\"\n        },\n        {\n          \"description\": \"The version number of the pipeline. A new pipeline always has a version number of 1. This number is incremented when a pipeline is updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"roleArn\",\n    \"stages\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-declaration-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PipelineDeclaration
---
