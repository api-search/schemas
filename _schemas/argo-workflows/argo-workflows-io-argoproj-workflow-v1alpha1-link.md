---
description: Link is a link to another app.
layout: schema
name: io.argoproj.workflow.v1alpha1.Link
properties_list:
- description: The name of the link, E.g. "Workflow Logs" or "Pod Logs"
  name: name
  type: string
- description: '"workflow", "pod", "pod-logs", "event-source-logs", "sensor-logs", "workflow-list" or "chat"'
  name: scope
  type: string
- description: Target attribute specifies where a linked document will be opened when a user clicks on a link. E.g. "_blank", "_self". If the target is _blank, it will open in a new tab.
  name: target
  type: string
- description: The URL. Can contain "${metadata.namespace}", "${metadata.name}", "${status.startedAt}", "${status.finishedAt}" or any other element in workflow yaml, e.g. "${io.argoproj.workflow.v1alpha1.metadata.an
  name: url
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-link-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-link
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Link
---
