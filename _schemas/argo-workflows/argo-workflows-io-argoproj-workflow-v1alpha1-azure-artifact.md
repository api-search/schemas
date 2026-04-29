---
description: AzureArtifact is the location of an Azure Storage artifact
layout: schema
name: io.argoproj.workflow.v1alpha1.AzureArtifact
properties_list:
- description: AccountKeySecret is the secret selector to the Azure Blob Storage account access key
  name: accountKeySecret
  type: object
- description: Blob is the blob name (i.e., path) in the container where the artifact resides
  name: blob
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
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-azure-artifact-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-azure-artifact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-azure-artifact-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.AzureArtifact\",\n  \"description\": \"AzureArtifact is the location of an Azure Storage artifact\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountKeySecret\": {\n      \"description\": \"AccountKeySecret is the secret selector to the Azure Blob Storage account access key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"blob\": {\n      \"description\": \"Blob is the blob name (i.e., path) in the container where the artifact resides\",\n      \"type\": \"string\"\n    },\n    \"container\": {\n      \"description\": \"Container is the container where resources will be stored\",\n      \"type\": \"string\"\n    },\n    \"endpoint\"\
  : {\n      \"description\": \"Endpoint is the service url associated with an account. It is most likely \\\"https://<ACCOUNT_NAME>.blob.core.windows.net\\\"\",\n      \"type\": \"string\"\n    },\n    \"useSDKCreds\": {\n      \"description\": \"UseSDKCreds tells the driver to figure out credentials based on sdk defaults.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"endpoint\",\n    \"container\",\n    \"blob\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-azure-artifact-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.AzureArtifact
---
