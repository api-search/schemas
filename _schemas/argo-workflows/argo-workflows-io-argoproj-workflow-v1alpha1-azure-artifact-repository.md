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
