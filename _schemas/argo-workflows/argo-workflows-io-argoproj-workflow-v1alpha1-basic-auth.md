---
description: BasicAuth describes the secret selectors required for basic authentication
layout: schema
name: io.argoproj.workflow.v1alpha1.BasicAuth
properties_list:
- description: PasswordSecret is the secret selector to the repository password
  name: passwordSecret
  type: object
- description: UsernameSecret is the secret selector to the repository username
  name: usernameSecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-basic-auth-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-basic-auth
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.BasicAuth
---
