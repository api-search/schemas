---
description: OSSArtifactRepository defines the controller configuration for an OSS artifact repository
layout: schema
name: io.argoproj.workflow.v1alpha1.OSSArtifactRepository
properties_list:
- description: AccessKeySecret is the secret selector to the bucket's access key
  name: accessKeySecret
  type: object
- description: Bucket is the name of the bucket
  name: bucket
  type: string
- description: CreateBucketIfNotPresent tells the driver to attempt to create the OSS bucket for output artifacts, if it doesn't exist
  name: createBucketIfNotPresent
  type: boolean
- description: Endpoint is the hostname of the bucket endpoint
  name: endpoint
  type: string
- description: KeyFormat defines the format of how to store keys and can reference workflow variables.
  name: keyFormat
  type: string
- description: LifecycleRule specifies how to manage bucket's lifecycle
  name: lifecycleRule
  type: object
- description: SecretKeySecret is the secret selector to the bucket's secret key
  name: secretKeySecret
  type: object
- description: 'SecurityToken is the user''s temporary security token. For more details, check out: https://www.alibabacloud.com/help/doc-detail/100624.htm'
  name: securityToken
  type: string
- description: UseSDKCreds tells the driver to figure out credentials based on sdk defaults.
  name: useSDKCreds
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-oss-artifact-repository-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-oss-artifact-repository
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.OSSArtifactRepository
---
