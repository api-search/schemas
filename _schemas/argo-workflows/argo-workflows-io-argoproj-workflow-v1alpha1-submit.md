---
description: io.argoproj.workflow.v1alpha1.Submit schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.Submit
properties_list:
- description: Arguments extracted from the event and then set as arguments to the workflow created.
  name: arguments
  type: object
- description: Metadata optional means to customize select fields of the workflow metadata
  name: metadata
  type: object
- description: WorkflowTemplateRef the workflow template to submit
  name: workflowTemplateRef
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-submit-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-submit
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-submit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-submit-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Submit\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.Submit schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arguments\": {\n      \"description\": \"Arguments extracted from the event and then set as arguments to the workflow created.\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Arguments\"\n    },\n    \"metadata\": {\n      \"description\": \"Metadata optional means to customize select fields of the workflow metadata\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.ObjectMeta\"\n    },\n    \"workflowTemplateRef\": {\n      \"description\": \"WorkflowTemplateRef the workflow template to submit\",\n\
  \      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.WorkflowTemplateRef\"\n    }\n  },\n  \"required\": [\n    \"workflowTemplateRef\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-submit-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Submit
---
