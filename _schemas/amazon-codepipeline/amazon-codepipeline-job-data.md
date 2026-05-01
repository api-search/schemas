---
description: Represents other information about a job required for a job worker to complete the job.
layout: schema
name: JobData
properties_list:
- description: ''
  name: actionTypeId
  type: object
- description: ''
  name: actionConfiguration
  type: object
- description: ''
  name: pipelineContext
  type: object
- description: ''
  name: inputArtifacts
  type: object
- description: ''
  name: outputArtifacts
  type: object
- description: ''
  name: artifactCredentials
  type: object
- description: ''
  name: continuationToken
  type: object
- description: ''
  name: encryptionKey
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-job-data-schema.json
slug: amazon-codepipeline-job-data
source_filename: amazon-codepipeline-job-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-job-data-schema.json\",\n  \"title\": \"JobData\",\n  \"description\": \"Represents other information about a job required for a job worker to complete the job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeId\"\n        },\n        {\n          \"description\": \"Represents information about an action type.\"\n        }\n      ]\n    },\n    \"actionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionConfiguration\"\n        },\n        {\n          \"description\": \"Represents information about an action configuration.\"\n        }\n      ]\n    },\n    \"pipelineContext\": {\n      \"allOf\": [\n        {\n         \
  \ \"$ref\": \"#/components/schemas/PipelineContext\"\n        },\n        {\n          \"description\": \"<p>Represents information about a pipeline to a job worker.</p> <note> <p>Includes <code>pipelineArn</code> and <code>pipelineExecutionId</code> for custom jobs.</p> </note>\"\n        }\n      ]\n    },\n    \"inputArtifacts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactList\"\n        },\n        {\n          \"description\": \"The artifact supplied to the job.\"\n        }\n      ]\n    },\n    \"outputArtifacts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactList\"\n        },\n        {\n          \"description\": \"The output of the job.\"\n        }\n      ]\n    },\n    \"artifactCredentials\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AWSSessionCredentials\"\n        },\n        {\n          \"description\": \"Represents an Amazon Web Services session credentials\
  \ object. These credentials are temporary credentials that are issued by Amazon Web Services Secure Token Service (STS). They can be used to access input and output artifacts in the S3 bucket used to store artifacts for the pipeline in CodePipeline.\"\n        }\n      ]\n    },\n    \"continuationToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContinuationToken\"\n        },\n        {\n          \"description\": \"A system-generated token, such as a deployment ID, required by a job to continue the job asynchronously.\"\n        }\n      ]\n    },\n    \"encryptionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionKey\"\n        },\n        {\n          \"description\": \"Represents information about the key used to encrypt data in the artifact store, such as an KMS key. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-job-data-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: JobData
---
