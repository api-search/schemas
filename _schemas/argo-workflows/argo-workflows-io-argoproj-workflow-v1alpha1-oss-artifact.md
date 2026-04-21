---
description: OSSArtifact is the location of an Alibaba Cloud OSS artifact
layout: schema
name: io.argoproj.workflow.v1alpha1.OSSArtifact
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
- description: Key is the path in the bucket where the artifact resides
  name: key
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
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-oss-artifact-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-oss-artifact
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.OSSArtifact
---
