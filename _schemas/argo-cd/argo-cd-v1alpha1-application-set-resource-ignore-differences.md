---
description: ApplicationSetResourceIgnoreDifferences configures how the ApplicationSet controller will ignore differences in live applications when applying changes from generated applications.
layout: schema
name: v1alpha1ApplicationSetResourceIgnoreDifferences
properties_list:
- description: JQPathExpressions is a list of JQ path expressions to fields to ignore differences for.
  name: jqPathExpressions
  type: array
- description: JSONPointers is a list of JSON pointers to fields to ignore differences for.
  name: jsonPointers
  type: array
- description: Name is the name of the application to ignore differences for. If not specified, the rule applies to all applications.
  name: name
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-resource-ignore-differences-schema.json
slug: argo-cd-v1alpha1-application-set-resource-ignore-differences
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetResourceIgnoreDifferences
---
