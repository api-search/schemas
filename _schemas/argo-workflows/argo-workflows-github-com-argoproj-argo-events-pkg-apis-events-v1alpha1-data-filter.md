---
description: DataFilter describes constraints and filters for event data.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.DataFilter
properties_list:
- description: Comparator compares the event data with a user given value. Can be ">=", ">", "=", "!=", "<", or "<=". Is optional, and if left blank treated as equality "=".
  name: comparator
  type: string
- description: Path is the JSONPath of the event's (JSON decoded) data key. Path is a series of keys separated by a dot. A key may contain wildcard characters '*' and '?'. To access an array value use the index as t
  name: path
  type: string
- description: ''
  name: template
  type: string
- description: ''
  name: type
  type: string
- description: Value is the allowed string values for this key. Booleans are parsed using strconv.ParseBool(), Numbers are parsed as float64 using strconv.ParseFloat(), Strings are treated as regular expressions, Ni
  name: value
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-data-filter-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-data-filter
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.DataFilter
---
