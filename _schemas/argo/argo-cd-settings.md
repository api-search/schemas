---
description: Argo CD server configuration settings.
layout: schema
name: Settings
properties_list:
- description: External URL of the Argo CD server.
  name: url
  type: string
- description: Dex OAuth provider configuration YAML.
  name: dexConfig
  type: string
- description: OIDC provider configuration YAML.
  name: oidcConfig
  type: string
- description: Whether application status badges are enabled.
  name: statusBadgeEnabled
  type: boolean
- description: Google Analytics tracking configuration.
  name: googleAnalytics
  type: object
- description: Help link configuration.
  name: help
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-settings-schema.json
slug: argo-cd-settings
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Settings
---
