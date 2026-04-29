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
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-oss-artifact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-oss-artifact-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.OSSArtifact\",\n  \"description\": \"OSSArtifact is the location of an Alibaba Cloud OSS artifact\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessKeySecret\": {\n      \"description\": \"AccessKeySecret is the secret selector to the bucket's access key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"bucket\": {\n      \"description\": \"Bucket is the name of the bucket\",\n      \"type\": \"string\"\n    },\n    \"createBucketIfNotPresent\": {\n      \"description\": \"CreateBucketIfNotPresent tells the driver to attempt to create the OSS bucket for output artifacts, if it doesn't exist\",\n      \"type\": \"boolean\"\n    },\n   \
  \ \"endpoint\": {\n      \"description\": \"Endpoint is the hostname of the bucket endpoint\",\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"description\": \"Key is the path in the bucket where the artifact resides\",\n      \"type\": \"string\"\n    },\n    \"lifecycleRule\": {\n      \"description\": \"LifecycleRule specifies how to manage bucket's lifecycle\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.OSSLifecycleRule\"\n    },\n    \"secretKeySecret\": {\n      \"description\": \"SecretKeySecret is the secret selector to the bucket's secret key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"securityToken\": {\n      \"description\": \"SecurityToken is the user's temporary security token. For more details, check out: https://www.alibabacloud.com/help/doc-detail/100624.htm\",\n      \"type\": \"string\"\n    },\n    \"useSDKCreds\": {\n      \"description\": \"UseSDKCreds tells the driver to figure out credentials\
  \ based on sdk defaults.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-oss-artifact-schema.json
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
