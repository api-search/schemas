---
description: Information about a pipeline.
layout: schema
name: PipelineMetadata
properties_list:
- description: ''
  name: pipelineArn
  type: object
- description: ''
  name: created
  type: object
- description: ''
  name: updated
  type: object
- description: ''
  name: pollingDisabledAt
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-pipeline-metadata-schema.json
slug: amazon-codepipeline-pipeline-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-metadata-schema.json\",\n  \"title\": \"PipelineMetadata\",\n  \"description\": \"Information about a pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the pipeline.\"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time the pipeline was created, in timestamp format.\"\n        }\n      ]\n    },\n    \"updated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n\
  \        {\n          \"description\": \"The date and time the pipeline was last updated, in timestamp format.\"\n        }\n      ]\n    },\n    \"pollingDisabledAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time that polling for source changes (periodic checks) was stopped for the pipeline, in timestamp format. You can migrate (update) a polling pipeline to use event-based change detection. For example, for a pipeline with a CodeCommit source, we recommend you migrate (update) your pipeline to use CloudWatch Events. To learn more, see <a href=\\\"https://docs.aws.amazon.com/codepipeline/latest/userguide/update-change-detection.html\\\">Migrate polling pipelines to use event-based change detection</a> in the CodePipeline User Guide.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-metadata-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PipelineMetadata
---
