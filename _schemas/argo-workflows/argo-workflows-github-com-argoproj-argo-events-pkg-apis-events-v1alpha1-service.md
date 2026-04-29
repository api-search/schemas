---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Service schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Service
properties_list:
- description: ''
  name: clusterIP
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: ports
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-service-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-service-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Service\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Service schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clusterIP\": {\n      \"type\": \"string\",\n      \"title\": \"clusterIP is the IP address of the service and is usually assigned\\nrandomly by the master. If an address is specified manually and is not in\\nuse by others, it will be allocated to the service; otherwise, creation\\nof the service will fail. This field can not be changed through updates.\\nValid values are \\\"None\\\", empty string (\\\"\\\"), or a valid IP address. \\\"None\\\"\\ncan be specified\
  \ for headless services when proxying is not required.\\nMore info: https://kubernetes.io/docs/concepts/services-networking/service/#virtual-ips-and-service-proxies\\n+optional\"\n    },\n    \"metadata\": {\n      \"title\": \"Metadata sets the pods's metadata, i.e. annotations and labels\\ndefault={annotations: {}, labels: {}}\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Metadata\"\n    },\n    \"ports\": {\n      \"type\": \"array\",\n      \"title\": \"The list of ports that are exposed by this ClusterIP service.\\n+patchMergeKey=port\\n+patchStrategy=merge\\n+listType=map\\n+listMapKey=port\\n+listMapKey=protocol\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.ServicePort\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-service-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.Service
---
