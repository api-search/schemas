---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameterSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameterSource
properties_list:
- description: 'ContextKey is the JSONPath of the event''s (JSON decoded) context key ContextKey is a series of keys separated by a dot. A key may contain wildcard characters ''*'' and ''?''. To access an array value use '
  name: contextKey
  type: string
- description: ''
  name: contextTemplate
  type: string
- description: DataKey is the JSONPath of the event's (JSON decoded) data key DataKey is a series of keys separated by a dot. A key may contain wildcard characters '*' and '?'. To access an array value use the index
  name: dataKey
  type: string
- description: ''
  name: dataTemplate
  type: string
- description: DependencyName refers to the name of the dependency. The event which is stored for this dependency is used as payload for the parameterization. Make sure to refer to one of the dependencies you have d
  name: dependencyName
  type: string
- description: ''
  name: useRawData
  type: boolean
- description: Value is the default literal value to use for this parameter source This is only used if the DataKey is invalid. If the DataKey is invalid and this is not defined, this param source will produce an er
  name: value
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-parameter-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-parameter-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameterSource
---
