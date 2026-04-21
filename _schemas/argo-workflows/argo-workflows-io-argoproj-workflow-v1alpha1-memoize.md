---
description: Memoize enables caching for the Outputs of the template.
layout: schema
name: io.argoproj.workflow.v1alpha1.Memoize
properties_list:
- description: Cache sets and configures the kind of cache
  name: cache
  type: object
- description: Key is the key to use as the caching key
  name: key
  type: string
- description: MaxAge is the maximum age (e.g. "180s", "24h") of an entry that is still considered valid. If an entry is older than the MaxAge, it will be ignored.
  name: maxAge
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-memoize-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-memoize
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Memoize
---
