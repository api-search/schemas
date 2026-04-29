---
description: AzureArtifactRepository defines the controller configuration for an Azure Blob Storage artifact repository
layout: schema
name: io.argoproj.workflow.v1alpha1.AzureArtifactRepository
properties_list:
- description: AccountKeySecret is the secret selector to the Azure Blob Storage account access key
  name: accountKeySecret
  type: object
- description: BlobNameFormat is defines the format of how to store blob names. Can reference workflow variables
  name: blobNameFormat
  type: string
- description: Container is the container where resources will be stored
  name: container
  type: string
- description: Endpoint is the service url associated with an account. It is most likely "https://<ACCOUNT_NAME>.blob.core.windows.net"
  name: endpoint
  type: string
- description: UseSDKCreds tells the driver to figure out credentials based on sdk defaults.
  name: useSDKCreds
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-azure-artifact-repository-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-azure-artifact-repository
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-azure-artifact-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-azure-artifact-repository-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.AzureArtifactRepository\",\n  \"description\": \"AzureArtifactRepository defines the controller configuration for an Azure Blob Storage artifact repository\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountKeySecret\": {\n      \"description\": \"AccountKeySecret is the secret selector to the Azure Blob Storage account access key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"blobNameFormat\": {\n      \"description\": \"BlobNameFormat is defines the format of how to store blob names. Can reference workflow variables\",\n      \"type\": \"string\"\n    },\n    \"container\": {\n      \"description\": \"Container is the\
  \ container where resources will be stored\",\n      \"type\": \"string\"\n    },\n    \"endpoint\": {\n      \"description\": \"Endpoint is the service url associated with an account. It is most likely \\\"https://<ACCOUNT_NAME>.blob.core.windows.net\\\"\",\n      \"type\": \"string\"\n    },\n    \"useSDKCreds\": {\n      \"description\": \"UseSDKCreds tells the driver to figure out credentials based on sdk defaults.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"endpoint\",\n    \"container\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-azure-artifact-repository-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.AzureArtifactRepository
---
