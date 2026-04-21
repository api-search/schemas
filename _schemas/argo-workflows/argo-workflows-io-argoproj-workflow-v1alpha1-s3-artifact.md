---
description: S3Artifact is the location of an S3 artifact
layout: schema
name: io.argoproj.workflow.v1alpha1.S3Artifact
properties_list:
- description: AccessKeySecret is the secret selector to the bucket's access key
  name: accessKeySecret
  type: object
- description: Bucket is the name of the bucket
  name: bucket
  type: string
- description: CASecret specifies the secret that contains the CA, used to verify the TLS connection
  name: caSecret
  type: object
- description: CreateBucketIfNotPresent tells the driver to attempt to create the S3 bucket for output artifacts, if it doesn't exist. Setting Enabled Encryption will apply either SSE-S3 to the bucket if KmsKeyId is
  name: createBucketIfNotPresent
  type: object
- description: ''
  name: encryptionOptions
  type: object
- description: Endpoint is the hostname of the bucket endpoint
  name: endpoint
  type: string
- description: Insecure will connect to the service with TLS
  name: insecure
  type: boolean
- description: Key is the key in the bucket where the artifact resides
  name: key
  type: string
- description: Region contains the optional bucket region
  name: region
  type: string
- description: RoleARN is the Amazon Resource Name (ARN) of the role to assume.
  name: roleARN
  type: string
- description: SecretKeySecret is the secret selector to the bucket's secret key
  name: secretKeySecret
  type: object
- description: SessionTokenSecret is used for ephemeral credentials like an IAM assume role or S3 access grant
  name: sessionTokenSecret
  type: object
- description: UseSDKCreds tells the driver to figure out credentials based on sdk defaults.
  name: useSDKCreds
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-s3-artifact-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-s3-artifact
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.S3Artifact
---
