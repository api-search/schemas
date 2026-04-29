---
description: S3EncryptionOptions used to determine encryption options during s3 operations
layout: schema
name: io.argoproj.workflow.v1alpha1.S3EncryptionOptions
properties_list:
- description: EnableEncryption tells the driver to encrypt objects if set to true. If kmsKeyId and serverSideCustomerKeySecret are not set, SSE-S3 will be used
  name: enableEncryption
  type: boolean
- description: KmsEncryptionContext is a json blob that contains an encryption context. See https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#encrypt_context for more information
  name: kmsEncryptionContext
  type: string
- description: KMSKeyId tells the driver to encrypt the object using the specified KMS Key.
  name: kmsKeyId
  type: string
- description: ServerSideCustomerKeySecret tells the driver to encrypt the output artifacts using SSE-C with the specified secret.
  name: serverSideCustomerKeySecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-s3-encryption-options-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-s3-encryption-options
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-s3-encryption-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-s3-encryption-options-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.S3EncryptionOptions\",\n  \"description\": \"S3EncryptionOptions used to determine encryption options during s3 operations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enableEncryption\": {\n      \"description\": \"EnableEncryption tells the driver to encrypt objects if set to true. If kmsKeyId and serverSideCustomerKeySecret are not set, SSE-S3 will be used\",\n      \"type\": \"boolean\"\n    },\n    \"kmsEncryptionContext\": {\n      \"description\": \"KmsEncryptionContext is a json blob that contains an encryption context. See https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#encrypt_context for more information\",\n      \"type\": \"string\"\n\
  \    },\n    \"kmsKeyId\": {\n      \"description\": \"KMSKeyId tells the driver to encrypt the object using the specified KMS Key.\",\n      \"type\": \"string\"\n    },\n    \"serverSideCustomerKeySecret\": {\n      \"description\": \"ServerSideCustomerKeySecret tells the driver to encrypt the output artifacts using SSE-C with the specified secret.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-s3-encryption-options-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.S3EncryptionOptions
---
