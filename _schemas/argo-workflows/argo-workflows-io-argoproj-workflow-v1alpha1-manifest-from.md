---
description: io.argoproj.workflow.v1alpha1.ManifestFrom schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.ManifestFrom
properties_list:
- description: Artifact contains the artifact to use
  name: artifact
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-manifest-from-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-manifest-from
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-manifest-from-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ManifestFrom\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.ManifestFrom schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"artifact\": {\n      \"description\": \"Artifact contains the artifact to use\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Artifact\"\n    }\n  },\n  \"required\": [\n    \"artifact\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-manifest-from-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ManifestFrom
---
