---
description: v1alpha1AWSAuthConfig schema from Argo CD API
layout: schema
name: v1alpha1AWSAuthConfig
properties_list:
- description: ''
  name: clusterName
  type: string
- description: Profile contains optional role ARN. If set then AWS IAM Authenticator uses the profile to perform cluster operations instead of the default AWS credential provider chain.
  name: profile
  type: string
- description: RoleARN contains optional role ARN. If set then AWS IAM Authenticator assume a role to perform cluster operations instead of the default AWS credential provider chain.
  name: roleARN
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-aws-auth-config-schema.json
slug: argo-cd-v1alpha1-aws-auth-config
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1AWSAuthConfig
---
