---
description: TTLStrategy is the strategy for the time to live depending on if the workflow succeeded or failed
layout: schema
name: io.argoproj.workflow.v1alpha1.TTLStrategy
properties_list:
- description: SecondsAfterCompletion is the number of seconds to live after completion
  name: secondsAfterCompletion
  type: integer
- description: SecondsAfterFailure is the number of seconds to live after failure
  name: secondsAfterFailure
  type: integer
- description: SecondsAfterSuccess is the number of seconds to live after success
  name: secondsAfterSuccess
  type: integer
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-ttl-strategy-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-ttl-strategy
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.TTLStrategy
---
