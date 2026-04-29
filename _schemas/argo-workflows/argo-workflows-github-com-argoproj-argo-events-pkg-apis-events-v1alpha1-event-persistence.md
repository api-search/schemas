---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventPersistence schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventPersistence
properties_list:
- description: ''
  name: catchup
  type: object
- description: ''
  name: configMap
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-persistence-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-persistence
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-persistence-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-persistence-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventPersistence\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventPersistence schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"catchup\": {\n      \"title\": \"Catchup enables to triggered the missed schedule when eventsource restarts\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.CatchupConfiguration\"\n    },\n    \"configMap\": {\n      \"title\": \"ConfigMap holds configmap details for persistence\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ConfigMapPersistence\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-event-persistence-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventPersistence
---
