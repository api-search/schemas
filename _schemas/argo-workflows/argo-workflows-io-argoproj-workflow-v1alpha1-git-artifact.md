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
