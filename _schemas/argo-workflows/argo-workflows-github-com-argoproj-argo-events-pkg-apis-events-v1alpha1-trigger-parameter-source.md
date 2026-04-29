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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-parameter-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameterSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameterSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contextKey\": {\n      \"description\": \"ContextKey is the JSONPath of the event's (JSON decoded) context key\\nContextKey is a series of keys separated by a dot. A key may contain wildcard characters '*' and '?'.\\nTo access an array value use the index as the key. The dot and wildcard characters can be escaped with '\\\\\\\\'.\\nSee https://github.com/tidwall/gjson#path-syntax for more information on how to\
  \ use this.\",\n      \"type\": \"string\"\n    },\n    \"contextTemplate\": {\n      \"type\": \"string\",\n      \"title\": \"ContextTemplate is a go-template for extracting a string from the event's context.\\nIf a ContextTemplate is provided with a ContextKey, the template will be evaluated first and fallback to the ContextKey.\\nThe templating follows the standard go-template syntax as well as sprig's extra functions.\\nSee https://pkg.go.dev/text/template and https://masterminds.github.io/sprig/\"\n    },\n    \"dataKey\": {\n      \"description\": \"DataKey is the JSONPath of the event's (JSON decoded) data key\\nDataKey is a series of keys separated by a dot. A key may contain wildcard characters '*' and '?'.\\nTo access an array value use the index as the key. The dot and wildcard characters can be escaped with '\\\\\\\\'.\\nSee https://github.com/tidwall/gjson#path-syntax for more information on how to use this.\",\n      \"type\": \"string\"\n    },\n    \"dataTemplate\": {\n\
  \      \"type\": \"string\",\n      \"title\": \"DataTemplate is a go-template for extracting a string from the event's data.\\nIf a DataTemplate is provided with a DataKey, the template will be evaluated first and fallback to the DataKey.\\nThe templating follows the standard go-template syntax as well as sprig's extra functions.\\nSee https://pkg.go.dev/text/template and https://masterminds.github.io/sprig/\"\n    },\n    \"dependencyName\": {\n      \"description\": \"DependencyName refers to the name of the dependency. The event which is stored for this dependency is used as payload\\nfor the parameterization. Make sure to refer to one of the dependencies you have defined under Dependencies list.\",\n      \"type\": \"string\"\n    },\n    \"useRawData\": {\n      \"type\": \"boolean\",\n      \"title\": \"UseRawData indicates if the value in an event at data key should be used without converting to string.\\nWhen true, a number, boolean, json or string parameter may be extracted.\
  \ When the field is unspecified, or explicitly\\nfalse, the behavior is to turn the extracted field into a string. (e.g. when set to true, the parameter\\n123 will resolve to the numerical type, but when false, or not provided, the string \\\"123\\\" will be resolved)\\n+optional\"\n    },\n    \"value\": {\n      \"description\": \"Value is the default literal value to use for this parameter source\\nThis is only used if the DataKey is invalid.\\nIf the DataKey is invalid and this is not defined, this param source will produce an error.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-parameter-source-schema.json
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
