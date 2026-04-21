---
description: PayloadField binds a value at path within the event payload against a name.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PayloadField
properties_list:
- description: Name acts as key that holds the value at the path.
  name: name
  type: string
- description: Path is the JSONPath of the event's (JSON decoded) data key Path is a series of keys separated by a dot. A key may contain wildcard characters '*' and '?'. To access an array value use the index as th
  name: path
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-payload-field-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-payload-field
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PayloadField
---
