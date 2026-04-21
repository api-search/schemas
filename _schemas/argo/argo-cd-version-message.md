---
description: Argo CD server version information.
layout: schema
name: VersionMessage
properties_list:
- description: Argo CD version string.
  name: Version
  type: string
- description: Build date.
  name: BuildDate
  type: string
- description: Git commit SHA of this build.
  name: GitCommit
  type: string
- description: Go language version used to build.
  name: GoVersion
  type: string
- description: Operating system and architecture.
  name: Platform
  type: string
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-version-message-schema.json
slug: argo-cd-version-message
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: VersionMessage
---
