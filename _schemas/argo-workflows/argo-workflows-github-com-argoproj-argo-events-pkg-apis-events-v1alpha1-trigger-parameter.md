---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter
properties_list:
- description: Dest is the JSONPath of a resource key. A path is a series of keys separated by a dot. The colon character can be escaped with '.' The -1 key can be used to append a value to an existing array. See ht
  name: dest
  type: string
- description: Operation is what to do with the existing value at Dest, whether to 'prepend', 'overwrite', or 'append' it.
  name: operation
  type: string
- description: ''
  name: src
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-parameter-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-parameter
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-parameter-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dest\": {\n      \"description\": \"Dest is the JSONPath of a resource key.\\nA path is a series of keys separated by a dot. The colon character can be escaped with '.'\\nThe -1 key can be used to append a value to an existing array.\\nSee https://github.com/tidwall/sjson#path-syntax for more information about how this is used.\",\n      \"type\": \"string\"\n    },\n    \"operation\": {\n      \"description\": \"Operation is what\
  \ to do with the existing value at Dest, whether to\\n'prepend', 'overwrite', or 'append' it.\",\n      \"type\": \"string\"\n    },\n    \"src\": {\n      \"title\": \"Src contains a source reference to the value of the parameter from a dependency\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameterSource\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-parameter-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter
---
