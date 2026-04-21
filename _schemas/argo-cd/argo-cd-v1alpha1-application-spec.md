---
description: ApplicationSpec represents desired application state. Contains link to repository with application definition and additional parameters link definition revision.
layout: schema
name: v1alpha1ApplicationSpec
properties_list:
- description: ''
  name: destination
  type: object
- description: ''
  name: ignoreDifferences
  type: array
- description: ''
  name: info
  type: array
- description: Project is a reference to the project this application belongs to. The empty string means that application belongs to the 'default' project.
  name: project
  type: string
- description: 'RevisionHistoryLimit limits the number of items kept in the application''s revision history, which is used for informational purposes as well as for rollbacks to previous versions. This should only be '
  name: revisionHistoryLimit
  type: integer
- description: ''
  name: source
  type: object
- description: ''
  name: sourceHydrator
  type: object
- description: ''
  name: sources
  type: array
- description: ''
  name: syncPolicy
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-spec-schema.json
slug: argo-cd-v1alpha1-application-spec
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSpec
---
