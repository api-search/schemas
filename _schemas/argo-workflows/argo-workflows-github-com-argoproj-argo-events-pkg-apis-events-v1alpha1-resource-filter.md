---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ResourceFilter schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ResourceFilter
properties_list:
- description: ''
  name: afterStart
  type: boolean
- description: ''
  name: createdBy
  type: object
- description: ''
  name: fields
  type: array
- description: ''
  name: labels
  type: array
- description: ''
  name: prefix
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-resource-filter-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-resource-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-resource-filter-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ResourceFilter\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ResourceFilter schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"afterStart\": {\n      \"type\": \"boolean\",\n      \"title\": \"If the resource is created after the start time then the event is treated as valid.\\n+optional\"\n    },\n    \"createdBy\": {\n      \"title\": \"If resource is created before the specified time then the event is treated as valid.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.Time\"\n    },\n    \"fields\": {\n      \"type\": \"array\"\
  ,\n      \"title\": \"Fields provide field filters similar to K8s field selector\\n(see https://kubernetes.io/docs/concepts/overview/working-with-objects/field-selectors/).\\nUnlike K8s field selector, it supports arbitrary fileds like \\\"spec.serviceAccountName\\\",\\nand the value could be a string or a regex.\\nSame as K8s field selector, operator \\\"=\\\", \\\"==\\\" and \\\"!=\\\" are supported.\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Selector\"\n      }\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"title\": \"Labels provide listing options to K8s API to watch resource/s.\\nRefer https://kubernetes.io/docs/concepts/overview/working-with-objects/label-selectors/ for more io.argoproj.workflow.v1alpha1.\\nUnlike K8s field selector, multiple values are passed as comma separated values instead of list of values.\\nEg: value: value1,value2.\\nSame as K8s label selector, operator \\\
  \"=\\\", \\\"==\\\", \\\"!=\\\", \\\"exists\\\", \\\"!\\\", \\\"notin\\\", \\\"in\\\", \\\"gt\\\" and \\\"lt\\\"\\nare supported\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Selector\"\n      }\n    },\n    \"prefix\": {\n      \"type\": \"string\",\n      \"title\": \"Prefix filter is applied on the resource name.\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-resource-filter-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ResourceFilter
---
