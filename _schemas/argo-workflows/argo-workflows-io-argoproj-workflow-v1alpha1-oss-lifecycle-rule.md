---
description: OSSLifecycleRule specifies how to manage bucket's lifecycle
layout: schema
name: io.argoproj.workflow.v1alpha1.OSSLifecycleRule
properties_list:
- description: MarkDeletionAfterDays is the number of days before we delete objects in the bucket
  name: markDeletionAfterDays
  type: integer
- description: MarkInfrequentAccessAfterDays is the number of days before we convert the objects in the bucket to Infrequent Access (IA) storage type
  name: markInfrequentAccessAfterDays
  type: integer
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-oss-lifecycle-rule-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-oss-lifecycle-rule
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.OSSLifecycleRule
---
