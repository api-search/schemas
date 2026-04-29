---
description: <p>The S3 bucket where artifacts for the pipeline are stored.</p> <note> <p>You must include either <code>artifactStore</code> or <code>artifactStores</code> in your pipeline, but you cannot use both. If you create a cross-region action in your pipeline, you must use <code>artifactStores</code>.</p> </note>
layout: schema
name: ArtifactStore
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: location
  type: object
- description: ''
  name: encryptionKey
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-artifact-store-schema.json
slug: amazon-codepipeline-artifact-store
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-artifact-store-schema.json\",\n  \"title\": \"ArtifactStore\",\n  \"description\": \"<p>The S3 bucket where artifacts for the pipeline are stored.</p> <note> <p>You must include either <code>artifactStore</code> or <code>artifactStores</code> in your pipeline, but you cannot use both. If you create a cross-region action in your pipeline, you must use <code>artifactStores</code>.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactStoreType\"\n        },\n        {\n          \"description\": \"The type of the artifact store, such as S3.\"\n        }\n      ]\n    },\n    \"location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactStoreLocation\"\
  \n        },\n        {\n          \"description\": \"The S3 bucket used for storing the artifacts for a pipeline. You can specify the name of an S3 bucket but not a folder in the bucket. A folder to contain the pipeline artifacts is created for you based on the name of the pipeline. You can use any S3 bucket in the same Amazon Web Services Region as the pipeline to store your pipeline artifacts.\"\n        }\n      ]\n    },\n    \"encryptionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionKey\"\n        },\n        {\n          \"description\": \"The encryption key used to encrypt the data in the artifact store, such as an Amazon Web Services Key Management Service key. If this is undefined, the default key for Amazon S3 is used.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"location\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-artifact-store-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ArtifactStore
---
