---
description: GitArtifact is the location of a git artifact
layout: schema
name: io.argoproj.workflow.v1alpha1.GitArtifact
properties_list:
- description: Branch is the branch to fetch when `SingleBranch` is enabled
  name: branch
  type: string
- description: Depth specifies clones/fetches should be shallow and include the given number of commits from the branch tip
  name: depth
  type: integer
- description: DisableSubmodules disables submodules during git clone
  name: disableSubmodules
  type: boolean
- description: Fetch specifies a number of refs that should be fetched before checkout
  name: fetch
  type: array
- description: InsecureIgnoreHostKey disables SSH strict host key checking during git clone
  name: insecureIgnoreHostKey
  type: boolean
- description: InsecureSkipTLS disables server certificate verification resulting in insecure HTTPS connections
  name: insecureSkipTLS
  type: boolean
- description: PasswordSecret is the secret selector to the repository password
  name: passwordSecret
  type: object
- description: Repo is the git repository
  name: repo
  type: string
- description: Revision is the git commit, tag, branch to checkout
  name: revision
  type: string
- description: SingleBranch enables single branch clone, using the `branch` parameter
  name: singleBranch
  type: boolean
- description: SSHPrivateKeySecret is the secret selector to the repository ssh private key
  name: sshPrivateKeySecret
  type: object
- description: UsernameSecret is the secret selector to the repository username
  name: usernameSecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-git-artifact-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-git-artifact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-git-artifact-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.GitArtifact\",\n  \"description\": \"GitArtifact is the location of a git artifact\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branch\": {\n      \"description\": \"Branch is the branch to fetch when `SingleBranch` is enabled\",\n      \"type\": \"string\"\n    },\n    \"depth\": {\n      \"description\": \"Depth specifies clones/fetches should be shallow and include the given number of commits from the branch tip\",\n      \"type\": \"integer\"\n    },\n    \"disableSubmodules\": {\n      \"description\": \"DisableSubmodules disables submodules during git clone\",\n      \"type\": \"boolean\"\n    },\n    \"fetch\": {\n      \"description\": \"Fetch specifies a number of refs\
  \ that should be fetched before checkout\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"insecureIgnoreHostKey\": {\n      \"description\": \"InsecureIgnoreHostKey disables SSH strict host key checking during git clone\",\n      \"type\": \"boolean\"\n    },\n    \"insecureSkipTLS\": {\n      \"description\": \"InsecureSkipTLS disables server certificate verification resulting in insecure HTTPS connections\",\n      \"type\": \"boolean\"\n    },\n    \"passwordSecret\": {\n      \"description\": \"PasswordSecret is the secret selector to the repository password\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"repo\": {\n      \"description\": \"Repo is the git repository\",\n      \"type\": \"string\"\n    },\n    \"revision\": {\n      \"description\": \"Revision is the git commit, tag, branch to checkout\",\n      \"type\": \"string\"\n    },\n    \"singleBranch\": {\n      \"description\"\
  : \"SingleBranch enables single branch clone, using the `branch` parameter\",\n      \"type\": \"boolean\"\n    },\n    \"sshPrivateKeySecret\": {\n      \"description\": \"SSHPrivateKeySecret is the secret selector to the repository ssh private key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"usernameSecret\": {\n      \"description\": \"UsernameSecret is the secret selector to the repository username\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  },\n  \"required\": [\n    \"repo\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-git-artifact-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.GitArtifact
---
