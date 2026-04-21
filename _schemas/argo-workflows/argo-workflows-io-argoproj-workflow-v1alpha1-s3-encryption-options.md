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
