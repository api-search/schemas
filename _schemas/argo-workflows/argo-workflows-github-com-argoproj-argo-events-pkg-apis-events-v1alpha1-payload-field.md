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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-payload-field-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PayloadField\",\n  \"description\": \"PayloadField binds a value at path within the event payload against a name.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Name acts as key that holds the value at the path.\",\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"description\": \"Path is the JSONPath of the event's (JSON decoded) data key\\nPath is a series of keys separated by a dot. A key may contain wildcard characters '*' and '?'.\\nTo access an array value use the index as the key. The dot and wildcard characters can be escaped with '\\\\\\\\'.\\nSee https://github.com/tidwall/gjson#path-syntax\
  \ for more information on how to use this.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-payload-field-schema.json
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
