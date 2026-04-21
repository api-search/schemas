---
description: Outputs hold parameters, artifacts, and results from a step
layout: schema
name: io.argoproj.workflow.v1alpha1.Outputs
properties_list:
- description: Artifacts holds the list of output artifacts produced by a step
  name: artifacts
  type: array
- description: ExitCode holds the exit code of a script template
  name: exitCode
  type: string
- description: Parameters holds the list of output parameters produced by a step
  name: parameters
  type: array
- description: Result holds the result (stdout) of a script or container template, or the response body of an HTTP template
  name: result
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-outputs-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-outputs
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Outputs
---
