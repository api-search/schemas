---
description: TemplateRef is a reference of template resource.
layout: schema
name: io.argoproj.workflow.v1alpha1.TemplateRef
properties_list:
- description: ClusterScope indicates the referred template is cluster scoped (i.e. a ClusterWorkflowTemplate).
  name: clusterScope
  type: boolean
- description: Name is the resource name of the template.
  name: name
  type: string
- description: Template is the name of referred template in the resource.
  name: template
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-template-ref-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-template-ref
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-template-ref-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-template-ref-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.TemplateRef\",\n  \"description\": \"TemplateRef is a reference of template resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clusterScope\": {\n      \"description\": \"ClusterScope indicates the referred template is cluster scoped (i.e. a ClusterWorkflowTemplate).\",\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"description\": \"Name is the resource name of the template.\",\n      \"type\": \"string\"\n    },\n    \"template\": {\n      \"description\": \"Template is the name of referred template in the resource.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-template-ref-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.TemplateRef
---
